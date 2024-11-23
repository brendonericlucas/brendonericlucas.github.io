Data infrastructure modernization (DIM) can be (at times, I think, intentionally) a _vauge_ phrase. 

Often, it tends to be a phrase which is bandied about after someone in a leadership position has finally become dissatisfied with paying folks for promised data driven insights that arrive stale - if they ever arrive at all - and who, when they start digging into what the likely cause of their poorly performing data teams is, find data professionals who seem to be 1) competent 2) committed and 3) exhausted, demoralized and overburdened by their work; note that I do _not_ necessarily suggest that leadership always recognizes all (or any) of 1 - 3, only that if they look closely, this is what they'll tend to find (but more on this below). 

Almost as often, it can be less indicative of particular concerns about an organization's data infrastructure than of some generalized FOMO. For example, "Company X is putting all of their data in the cloud. Why aren't we doing that? When are we going to do that?". 

And speaking of the cloud, this is another thing that data infrastructure modernization can often encompass. Namely, efforts to shift some large part - or all - of an organization's data platform to cloud based resources and services. 

From my experiences in industry (and the experiences of many others...stories of failed data warehousing projects, which are often a core component of DIM projects, are legion), DIM projects are often doomed to failure pretty much as soon as, or even before, they start. If data _really is_ the new oil, then these projects are a bit akin to flooding the ocean with crude instead of piping it, processing it, and exporting it. That is to say, very messy and very, _very_ wasteful. 

Given the constant deluge of data which organizations today are tasked with managing, it behooves us to ask _why_ so many DIM projects will fail. Here are some of the recurring culprits I've seen in industry while working at organizations public and private, small and large. 

---

## There is no such thing as a "Data Infrastructure Modernization Project"

Because technology is constantly changing, and data infrastructure needs to change with it. I once had a (non-technical) manager who asked me - repeatedly - when the data warehouse we were building was going to be "done". I tried to explain (and was, I think, eventually successful in doing so...eventually!) that it wasn't ever going to be in anything like a final state. The most we could reasonably aim for was to have a sliding window where data assets outside that window and prior to it were considered fixed and immutable within the data warehouse (and even that was a bit of a gloss). 

Data modernization efforts, in order to be really successful, need to be continual and ongoing. On a regular (at least annual) basis, organizations need to assess the current data technology landscape and determine and prioritize which parts of it they want to absorb into their own data ecosystem (as well as which parts of their existing infrastructure they can dispense with...it's the ship of Theseus we're sailing here). This is the correct way to do DIM. Think of it as akin to CI/CD, but for the base components of your data infrastructure rather than application source code. 

Organizations which fail to devote sufficient resources to continual improvement of their data infrastructure are those which wind up having to take on DIM "projects", or concerted pushes to do in a relatively short time what had better been done gradually and incrementally over a longer term. 

## You can't always get what you want (and even if you try - sometimes - you can't get what you need)
It may seem a truism, but where you start out in your efforts to modernize your data infrastructure largely limits where you can expect to wind up, at least in the short - medium term. 

If you've negelected your data systems - or put off investing in them - for some time, there probably isn't any amount of heroics which is going to put you in a position to make up for all of that lost time in a 12 - 24 month timeframe (or a 36 - 48 month timeframe, for that matter). 

Upgrading data systems is a genuine _investment_. And like most traditional investments, some period of time will need to elapse before those investments start delivering returns. I've also seen these "ramp up" efforts fail due to an "everything all at once approach" that tries to impose a uniform set of technologies and way of working across a large org with considerable diversity respecting team sizes, team skill sets, team goals and business alignment, etc. The tendancy to adopt this sort of approach is understandable given the impetus for taking up this variety of work in the first place. But there are serious risks to morale and team cohesion lying along this path, and problems in those areas can easily overwhelm efforts to solve the technology obsolescence problem an organization ostensibly set out to solve in the first place. 

---


## You have too much (and the wrong kind of) middle management
Technical teams need technical leaders. Period. Full stop. End of Story. But they also need _people_ leaders. 

Often, the glib assumption we seem to make is that someone who comes up short in the former respect must excel in the latter respect. But actually, more of the really effective people leaders of the technical teams I've been on have also been technically quite capable. 

Sometimes, less technical leaders may find themselves leading more technical teams because the nature of the team has changed over time, going from a less technical data team to a more technical data team. In order to be really effective, those leaders need to do their part to up-skill themselves. If they can't - or just won't - then they should be given the option to make a lateral move to a team where their relative paucity of technical prowess won't be such an encumberance, or released if they decline. 

Having many mediocre middle managers - i.e., managers who are not technically good, and who are casually assumed to be better at the soft skills side of management just _because_ they are known to not be tehcnically good - can kill a data infrastructure modernization effort where it stands. Large scale data migration projects are complex beasts. Things can go wrong, and they will. A leader needs to be able to roll up their sleeves and help steer the team through rough technical seas. If you have middle managers who have no idea what's going on within their teams - and think they don't need to, because "that's what the SMEs are for" - then you have too many and / or the wrong kind of middle management. 

An important rider here is that no one wants to work for a _weak leader_ either, regardless of how technically good they might be. If they don't have the spine to push back against unreasonable asks or hairbrained ideas, don't adopt a protective stance towards their team, don't value or respect their team except as a means of their own enrichment or survivial - then here, too, your modernization effort will likely fail. 

---

## You have poor (or no) engineering culture
I've worked on teams where there was quite literally no code review (on at least one occasion, because there just *wasn't* anyone who could do the reviewing). I've also worked on teams where there was no real documentation, and where documenting one's work just never really 'caught on' as a best practice. These teams both had poor - or completely absent - engineering culture. 

There's a real and genuine difference between mature, professional engineering teams and teams comprised of what are effectively accomplished amateurs. 

Professional engineering teams are aware of and try to follow industry best practices (often tinkering with them around the margins to adapt them to their particular situations). They find ways to foster meaningful collaboration. They bake *meaningful* and right-sized safeguards and quality checks into their development workflows and they resist process for process's sake. They embrace and celebrate clear and detailed documentation and aren't afraid to show their work. They also understand the place of agile and traditional development methods in delivering value for an organization. 

Perhaps most importantly, they don't tolerate or support an environment in which *every single solution* is a uniquely creative solution. Because it's highly unlikely, especially in the sort of org which needs to undertake a DIM effort, that the problems you're trying to solve are really so *sui generis* that the only way to approach them is to reinvent the wheel. Other folks have tackled these challenges before. They've recorded what worked and what didn't work. If a team dives into a DIM problem without first taking the time to familiarize itself with the current collective wisdom reagarding how to solve a problem of the sort they're faced with, then they're not approaching the problem as engineering professionals. 

Poor or non-existint engineering culture is yet another threat to a sucessful data infrastructure modernization effort. 

---

## You have poor team culture / are failing at recruitment, mentoring, and psychological safety
Poor team culture can hinder the pace of new technology adoption, which can - over time - dampen team morale as the value the team is able to demonstrate begins to decline, or the amount of effort required to deliver that value increases relative to the requirements experienced by teams who work with more modern data stacks. 

The biggest issues I've seen in industry here are failures to recruit, develop, and retain talent. The main culprits that I've seen here are the ones below. 

### You've been overrelying on contractor labor
Call me a pessimist, but relying almost soley on outside contractors to do the actual _work_ required to build the data products your business needs while maintaining a smaller staff of FTEs for the sole purpose of managing those contractors (and maintaining the data systems they built once they've moved on) has never seemed like a sound way to run a technology team to me. 

There are a number of things that tend to happen when teams operate in this fashion, none of which bode well for an organization's data infrastructure. 

For one thing, teams which operate in this fashion tend not to develop any real capability to develop internal talent. Contractors, on this model, are (for better or worse) treated basically as completely disposable technical resources. If a contractor has an issue completing a task, teams which operate in this way don't tend to bother much with trying to determine _why_. The contractor is simply replaced. 

This loop of hiring and firing contractors when the work isn't getting done might go through several iterations before someone finally completes the project. It might be that that person really was much more capable than the folks who came before them, and that's why they were able to succeed where their predecessors failed. Or it might simply be that each of the previous folks moved the ball forward a good measure, advancing against unrealistic timelines and unreasonable expectations, so that the last person who worked on the project was handed something that was already within striking distance of "done". Either way, there's really nothing to celebrate here. When the last person is gone, much of their knowledge will depart with them. And the folks who are left - the "managers" - won't have any insight into the actual issues which caused the project to drag. So those are two opportuities to develop internal talent wasted: one on the contractor, and one on the FTEs who managed them. 

Ultimately, this sort of approach speaks to a lazy and stagnant management culture on a technology team. 

Another issue here is the one already alluded to above. Namely, the issue of _knowledge continuity_. Knowledge of how things work on a technical level is an asset to an org. Overrelying on contractors is a sure way to make certain that that knowledge is patchy and diffuse. It simply doesn't work in the long run. 


### You think hiring a bunch of recent college grads / master's students is going to save you
Another thing which often happens to teams who face significant culture challenges of the sort described above is that the techincal skills of their FTEs atrophy through disuse. When this happens, there is often a push to try to 'solve' the problem of not having anyone on staff who actually knows what they're doing by hiring a bunch of recent graduates to 'bring the team up to speed'. The charitable interpretation here is that the FTEs are hoping that the younger folks can teach them the new technologies they haven't bothered to keep up with, while they teach them the ins and outs of the legacy data systems they'll eventually be responsible for helping to 'modernize'. 

This rarely ever works. For one thing, the FTEs often don't really _know_ their own systems as well as the length of their tenure with the team might suggest they ought to. Remember, all they did was 'manage' the contractors who actually built all this stuff. They often simply _can't_ provide the missing technical knowledge required to get the newly hired folks to the point where they're able to be productive quickly. For another thing, the non-management FTEs are probably not the most motivated to learn the new skills the new hires were hired to teach. They've mostly been doing dreadfully boring maintenance / production support tasks to keep things other people built running, and they've by now become very accustomed to the by-rote quality of their job. 

Letting cultural rot of this sort take hold within a team is tantamount to digging a deep hole over a long period of time. It takes years of consistently poor leadership to make something like this happen. And it cannot be fixed overnight, even with an army of bright recent graduates and hardworking interns. 

---

## You are too focused on "just getting the work done"
This brings us to the last of the major causes of the failure of data infrastructure modernization efforts: an excessive devotion to 'pragmatism' and manual effort. 

No one gets into technology to perform boring and repetitive tasks which can be automated. But building proper automation takes time. It's another sort of investment. Teams who don't want to make that investment (often because they feel that automation and efficiency are _dangerous_ to their continued existence) birth data roles that can - at their very worst - feel like glorifed clerical postions (Not that there's anything wrong with working in a clerical position! There isn't! It's just not what technologically inclined folks like to do.) 

To build a team that can build and maintain a solid infrastructure, you need to pay almost as much attention to _how_ the work is getting done as to whether it is getting done. And this includes, of course, your data infrastructure modernization efforts themselves. 
