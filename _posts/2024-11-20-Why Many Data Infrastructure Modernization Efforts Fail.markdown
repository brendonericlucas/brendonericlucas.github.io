# IN PROGRESS

Data infrastructure modernization (DIM) can be (at times, I think, intentionally) a _vauge_ term. 

Often, it tends to be a phrase which is bandied about after someone in a leadership position has finally become dissatisfied with paying folks for promised data driven insights that arrive stale - if they ever arrive at all - and who, when they start digging into what the likely cause of their poor performing data teams is, find data professionals who seem to be 1) competent 2) committed and 3) exhausted, demoralized and overburdened by their work; note that I do _not_ necessarily suggest that leadership always recognizes all (or any) of 1 - 3, only that if they look closely, this is what they'll tend to find (but more on this below). 

Almost as often, it can be less indicative of particular concerns about an organization's data infrastructure than of some generalized FOMO. For example, "Company X is putting all of their data in the cloud. Why aren't we doing that? When are we going to do that?". 

And speaking of the cloud, this is another thing that data infrastructure modernization can often encompass. Namely, efforts to shift some large part - or all - of an organization's data platform to cloud based resources. 

From my experiences in industry (and the experiences of many others...stories of failed data warehousing projects, which are often a core component of DIM projects, are legion), DIM projects are often doomed to failure pretty much as soon, or even before, they start. If data _really is_ the new oil, then these projects are a bit akin to flooding the ocean with crude instead of piping it, processing it, and exporting it. That is to say, very messy and very, _very_ wasteful. 

Given the constant deluge of data which organizations today are tasked with managing, it behooves us to ask _why_ so many DIM projects will fail. Here are some of the recurring culprits I've seen in industry while working at organizations public and private, small and large. 

---

## There is no such thing as a "Data Infrastructure Modernization Project"

Because technology is constantly changing, and data infrastructure needs to change with it. I once had a (non-technical) manager who asked me - repeatedly - when the data warehouse we were building was going to be "done". I tried to explain (and was, I think, eventually successful in doing so...eventually!) that it wasn't ever going to be in anything like a final state. The most we could reasonably aim for was to have a sliding window where data assets outside that window and prior to it were considered fixed and immutable within the data warehouse (and even that was a bit of a gloss). 

Data modernization efforts, in order to be really successful, need to be continual and ongoing. On a regular (at least annual) basis, organizations need to assess the current data technology landscape and determine and prioritize which parts of it they want to absorb into their own data ecosystem. This is the correct way to do DMI. Think of it as akin to CI/CD, but for the base components of your data infrastructure rather than application code. 

Organizations which fail to devote sufficient resources to continual improvement of their data infrastructure are those which wind up having to take on DIM "projects", or concerted pushes to do in a relatively short time what they had better been doing gradually over the long term. 


