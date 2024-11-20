# IN PROGRESS

Data infrastructure modernization (DIM) can be (at times, I think, intentionally) a _vauge_ term. 

Often, it tends to be a phrase which is bandied about after someone in a leadership position has finally become dissatisfied with paying folks for promised data driven insights that arrive stale - if they ever arrive at all - and who, when they start digging into what the likely cause of their poorly performing data teams is, find data professionals who seem to be 1) competent 2) committed and 3) exhausted, demoralized and overburdened by their work; note that I do _not_ necessarily suggest that leadership always recognizes all (or any) of 1 - 3, only that if they look closely, this is what they'll tend to find (but more on this below). 

Almost as often, it can be less indicative of particular concerns about an organization's data infrastructure than of some generalized FOMO. For example, "Company X is putting all of their data in the cloud. Why aren't we doing that? When are we going to do that?". 

And speaking of the cloud, this is another thing that data infrastructure modernization can often encompass. Namely, efforts to shift some large part - or all - of an organization's data platform to cloud based resources and services. 

From my experiences in industry (and the experiences of many others...stories of failed data warehousing projects, which are often a core component of DIM projects, are legion), DIM projects are often doomed to failure pretty much as soon, or even before, they start. If data _really is_ the new oil, then these projects are a bit akin to flooding the ocean with crude instead of piping it, processing it, and exporting it. That is to say, very messy and very, _very_ wasteful. 

Given the constant deluge of data which organizations today are tasked with managing, it behooves us to ask _why_ so many DIM projects will fail. Here are some of the recurring culprits I've seen in industry while working at organizations public and private, small and large. 

---

## There is no such thing as a "Data Infrastructure Modernization Project"

Because technology is constantly changing, and data infrastructure needs to change with it. I once had a (non-technical) manager who asked me - repeatedly - when the data warehouse we were building was going to be "done". I tried to explain (and was, I think, eventually successful in doing so...eventually!) that it wasn't ever going to be in anything like a final state. The most we could reasonably aim for was to have a sliding window where data assets outside that window and prior to it were considered fixed and immutable within the data warehouse (and even that was a bit of a gloss). 

Data modernization efforts, in order to be really successful, need to be continual and ongoing. On a regular (at least annual) basis, organizations need to assess the current data technology landscape and determine and prioritize which parts of it they want to absorb into their own data ecosystem. This is the correct way to do DIM. Think of it as akin to CI/CD, but for the base components of your data infrastructure rather than application source code. 

Organizations which fail to devote sufficient resources to continual improvement of their data infrastructure are those which wind up having to take on DIM "projects", or concerted pushes to do in a relatively short time what had better been done gradually and incrementally over a longer term. 

## You can't always get what you want (and even if you try - sometimes - you can't get what you need)
It may seem a truism, but where you start out in your efforts to modernize your data infrastructure largely limits where you can expect to wind up, at least in the short - medium term. 

If you've negelected your data systems - or put off investing in them - for some time, there probably isn't any amount of heroics which is going to put you in a position to make up for all of that lost time in a 12 - 24 month timeframe (or a 36 - 48 month timeframe, for that matter). 

Upgrading data systems is a genuine _investment_. And like most traditional investments, some period of time will need to elapse before those investments start delivering returns. I've also seen these "ramp up" efforts fail due to an "everything all at once approach" that tries to impose a uniform set of technologies and way of working across a large org evidencing considerable diversity respecting team sizes, team skill sets, team goals and business alignment, etc. The tendancy to adopt this sort of approach is understandable given the impetus for taking up this variety of work in the first place. But there are serious risks to morale and team cohesion lying along this path, and problems in those areas can easily overwhelm efforts to solve the technology obsolescence problem an organization really set out to solve in the first place. 

## You have too much (and the wrong kind of) middle management
Technical teams need technical leaders. Period. Full stop. End of Story. But they also need _people_ leaders. 

Often, the glib assumption we seem to make is that someone who comes up short in the former respect must excel in the latter respect. But actually, more of the really effective people leaders of the technical teams I've been on have also been technically quite capable. 

Sometimes, less technical leaders may find themselves leading more technical teams because the nature of the team has changed over time, going from a less technical data team to a more technical data team. In order to be really effective, those leaders need to do their part to up-skill themselves. If they can't - or just won't - then they should be given the option to make a lateral move to a team where their relative paucity of technical prowess won't be such an encumberance, or released if they decline. 

Having many mediocre middle managers - i.e., managers who are not technically good, and who are casually assumed to be better at the soft skills side of management just _because_ they are known to not be tehcnically good - can kill a data modernization effort where it stands. Large scale data migration projects are complex beasts. Things can go wrong, and they will. A leader needs to be able to roll up their sleeves and help steer the team through rough technical seas. If you have middle managers who have no idea what's going on in their teams - and think they don't need to, because "that's what the SMEs are for" - then you have too many and / or the wrong kind of middle management. 

An important rider here is that no one wants to work for a _weak leader_ either, regardless of how technically good they might be. If they don't have the spine to push back against unreasonable asks or hairbrained ideas, don't adopt a protective stance towards their team, don't value or respect their team except as a means of their own enrichment or survivial - then here, too, your modernization effort will likely fail. 

## You have poor (or no) engineering culture


## You have poor team culture / are failing at recruitment, mentoring, and psychological safety


### You've been overrelying on contractor labor


### You think hiring a bunch of recent college grads / master's students is going to save you


## You are too focused on "just getting the work done"

