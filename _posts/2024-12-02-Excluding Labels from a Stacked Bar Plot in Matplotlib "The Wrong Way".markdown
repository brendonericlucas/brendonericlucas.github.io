# The Scenario

Recently, I wanted to produce a simple stacked barchart for a NLI classification problem using [matplotlib](https://matplotlib.org/), and wanted to label the bars with the corresponding counts using the built-in [`bar_label(...)`](https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.bar_label.html) method.

The classication problem was a standard, three class natural language inference problem. Given a premise and a hypothesis, the model was to determine which of three lables applied: 0 (for entailment), 1 (for neutrality), or 2 (for contradiction). 

The stacked barcharts were to be a representation of the error set (i.e., set of all misclassified instances) over the test set. For each gold label, we want to construct a bar whose height is equal to the total count of the misclassified instances having that gold label, and whose components show the counts of each of the other two (incorrect) labels which the model actually assigned to each misclassified instance with the given gold label. The end result would look like the below:

![Stacked Bar Chart](/docs/assets/images/tm_sbc.png)

# The Problem

An easy way to add the labels in the above so that they look good with minimal coding / without having to futz with low-level annotation methods is to use the `bar_label` method referenced above. The tradeoff here is the ususal one...less code written, less time taken to produce a desired visualization, and this comes at the cost of less flexibility. 

The issue I was having was that there are _three_ class labels, but clearly only 2 of the three should be displayed on any particular bar (because the third will agree with the gold label, and so there will be zero instances associated with it). 

Using the below code, all three labels are displayed, including the label associated with the gold label, which is wrong (and looks funny): 

    for predicted_label, predicted_label_count in predicted_label_counts.items():
        p = ax.bar(gold_label, predicted_label_count, width, label=predicted_label, bottom=bottom)
        bottom += predicted_label_count

        ax.bar_label(p, label_type='center')

This is 95% of what we want here, aside from the gold labels showing up. 

# The Correct Solution
I believe the "correct" way to address this might be to fallback to lower-level [annotation](https://matplotlib.org/stable/users/explain/text/annotations.html) methods, or maybe to invoke the `remove( )` method on one of the bar [artists](https://matplotlib.org/stable/api/artist_api.html#matplotlib.artist.Artist) to strip out the offending gold label annotation that the `bar_label( )` method adds by default. 

# The Workaround
For me, neither of the above approaches seemed "worth the squeeze" given that I already had 95% of what I needed, and just needed to close the gap on that last 5% in order to produce the visualization above. 

Fortunately, there's a "quick and dirty" fix for this issue when you know the count values you want to exclude ahead of your call to the `bar_label( )` method _and_ you're invoking the `bar_label( )` method that belongs to the `axes` library. 

If you look at the source for the `bar_label( )` method, you'll find the below lines right before the method returns: 

```
annotation = self.annotate(lbl, xy, xytext, textcoords="offset points",
                           ha=ha, va=va, **kwargs)
annotations.append(annotation)
```

It turns out that `lbl` actually holds the count value which the annotate method will add to the bars when it's called within `bar_plot( )`. 

For our use case, we want to exclude the values of `lbl` equal to 0. The most straightforward way to do that is to add a check before the call to `self.annotate` to ensure that the annotation is created and added to the `annotations` container only if the `lbl` value is greater than zero. 

With that change, the above becomes: 

```
if lbl not in (0, '0'):
  # only add annotations if the count - given by lbl - is greater than 0
  annotation = self.annotate(lbl, xy, xytext, textcoords="offset points",
                             ha=ha, va=va, **kwargs)
  annotations.append(annotation)
```

With that one simple change, we get the stacked bar chart we actually wanted, and without having to mess with creating annotations ourselves or working with artists. 
