# The Scenario

Recently, I wanted to produce a simple stacked barchart for a NLI classification problem using [matplotlib](https://matplotlib.org/), and wanted to label the bars with the corresponding counts using the built-in [`bar_label(...)`](https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.bar_label.html) method.

The classication problem was a standard, three class natural language inference problem. Given a premise and a hypothesis, the model was to determine which of three lables applied: 0 (for entaliment), 1 (for netrality), or 2 (for contradiction). The stacked barcharts were to be a representation of the error set (i.e., set of all misclassified instances) over the testing set. For each gold label, we want to construct a bar whose height is equal to the total count of the misclassified instances having that gold lable, and whose components show the counts of each of the other two (incorrect) lables which the model actually assigned to each misclassified instance with the given gold label. The end result would look like the below:

![Stacked Bar Chart](/docs/assets/images/tm_sbc.png)


