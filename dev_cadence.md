### Development Model and Cadence

__Continuous Delivery__    

We follow a continuous delivery model.  This means, all changes are merged into master (more info about branching strategy [here](branching.md)).  This pretty much can happen at any time, and we shouldn't ever be afraid of "pushing to production".  Even if there's a bigger change going in, we should be taking bit sized chunks in implementing it.  This model almost forces us to think of problems in smaller consumable chunks, as you never want to have a branch or deployment that has been under development for too long without merging into branch and ran in production

__Weekly Sprints__   

It's best to have a "sign post" to let you know where you're going.  This is the purpose of our weekly sprints.  The sprints aren't meant to be "release" points, but a milestone target for us to hit.  These should be reasonable things we want to do and the Trello board should be broken up in these lists:

* Sprint XXX Retro (after the sprint is finished) - What we learned, what we want to run post-mortem on
* Sprint XXX Milestone - High level target we're shooting for this sprint
* This Sprint - Items to do for this sprint, including ones in-progress.  If there's a "member" associated, it's assigned or been worked on
* Sprint XXX Completed - Completed tasks for the specified sprint sprint
* Backlog - Items waiting to be assigned to an upcoming sprint
* Teaching Tuesdays - Lessons to be shared by team members
* Business / Misc - Items we need to work on from a business prospective
* Tabled - Things we need to do but are tabled for now, as we don't need to do it "right this minute".  However, it should be done within the next few sprints
* Fault Tolerance - Things to consider longer term when it comes to scaling, "long" running tabled items

__GitHub Issues__

So, the big question is, when to use Trello over GitHub issues?  We debated this, and in the end we are using both.  Trello for the "bigger" items, and GitHub for specific bugs and enhancements we need to fix.  GitHub issues should be created for each PR, and in that case, a "card" on Trello could make up multiple pull requests.

__Hackathons__    

We hold two types of hackathons.  One is a "business related" hackathon, while another is a "random idea hackathon".  We try to hold hackathons every 4-5 sprints.  The "business related" is something that is related to our business, but may not be specific to the platform we're building. 

###Trello Board Management

Here are some simple rules for our board management

* We have a ["Main Sprint Board"](https://trello.com/b/WiYowf0f/main-sprint-board) where all current activies go in
* For each new sprint, two lists are created, a Sprint xx Milestone list, and Sprint xx Completed list.  The Milestone list is the targets we have for this particular sprint, and then all completed todos go into the completed list.
* Don't try to stuff too much, if there's over 20 todos, we might have over-stuffed it
* Things that don't get done, should be moved to the next sprint, or moved back to Backlog, or put in the ["Sprint Graveyard"](https://trello.com/b/QQc4J4RQ/sprint-graveyard).  The idea of the graveyard is to put items that don't make sense after we've gotten a bit into it or something we've tabled indefinitely.

__Sprint Completion__

* Move Completed tasks to the ["Completed Board"](https://trello.com/b/jgvsWCzu/completed)
* Look at the "This Sprint" list and see where we're at, and if they are completed or not
* Look at Milestones and determine if we've met them and any that haven't been met, should be moved to the next Sprint's milestone (unless it was deemed invalid)
* Complete a Retro for the finishing Sprint, and move it to the Completed Board
* Review the backlog to see what else should be pulled into the "This Sprint" list.

__BrighterlinkIO Public Board__

We have a public trello [board](https://trello.com/b/zHSsSxGQ/brighterlink-io).  This is a public-facing board so we don't want to get into too much of the nitty gritty, but it's good to give some high level updates.  Thus, after each sprint, we should move over the items that make sense and then create new ones as needed.


### Useful Links

[Brightergy Trello](https://trello.com/brightergy2)    
[Hackathon](https://trello.com/b/cTP0Grnn/hackathon)    
