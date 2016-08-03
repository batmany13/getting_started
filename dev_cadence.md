### Development Model and Cadence

__Overview__

We follow a near continuous delivery model.  The "near" is due to the fact we haven't fully automated our Heroku Pipeline for deploying from staging to production.  Our [branching strategy](branching.md) and pipeline allows us to test individual branches, and as changes are merged into master, it's automatically deployed to a staging environment, where we run additional system tests.  Then, the changes from staging are pushed to prod on a semi regular basis (after everything on staging looks right).  We are moving towards continouous, and hopefully we can take out this section soon, but the general idea of continuous or near continous delivery models is to never be afraid to push to production, design and implement in bit sized chunks and never be under development or running in prod for too long.

__BrighterLink Roadmap__    

This lives in ["Trello"](https://trello.com/b/zHSsSxGQ/brighterlink-roadmap).  This gives you a high level overview of what capabilities we want to add, and is usually a couple of months out.  This board is meant for non-technical people, and is our main interaction point with business leaders within Brightergy.  We can then derive our weekly sprints and individual features/bugs from this list.

__Weekly Sprints__   

These live in milestones within GitHub.  The team will translate the items identified in the BrighterLink roadmap into weekly milestones and then individual GitHub issues that represent the technical work needed to accomplish the goal.  Also, on-going maintenance, bug fixes, clean up and misc issues are stored there as well.  Typically a milestone is broken up into 4 weekly intervals.  The format is the name of the monthly Milestone (currently after local beers) and then the week #.  So for sample you'll see `Tank7 - Sprint 1`, Tank7 being the monthly release that spanned 7/11/2016 - 8/7/2016.

__Hackathons__    

Building great software is fun, but we also believe in "opening the mind" up to new ideas and things.  We do this with hackathons, an event where developers get to work on various things that are outside of their normal day to day work.  We hold two types of hackathons.  One is a "business related" hackathon, while another is a "green field hackathon".  The first type is something that is tangerially related to our core business, but not something we're looking to do or would want to work on right away.  It also could be using our service as a customer and building something on top of it.  The second type is completely open and could be any idea thats randomly popped into our minds.  We try to hold hackathons every 2 or 3 milestones.

### Useful Links

[Brightergy's Trello account](https://trello.com/brightergy2)    
[Hackathon Board](https://trello.com/b/cTP0Grnn/hackathon)    
[GitHub Miletones for BrighterLink API](https://github.com/Brightergy/brighterlink-io/milestones)   
[GitHub Milestones for BrighterLink UI](https://github.com/Brightergy/brighterlink-ui/milestones)   
[GitHub Milestones for Digi](https://github.com/Brightergy/digi_gateway/milestones)   