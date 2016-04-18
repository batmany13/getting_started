### Development Model and Cadence

__Continuous Delivery__    

We follow a continuous delivery model.  This means, all changes that are merged into master (more info about branching strategy [here](branching.md)).  This pretty much can happen at any time, and we shouldn't ever be afraid of "pushing to production".  Even if there's a bigger change going in, we should be taking bit sized chunks in implementing it.  This model almost forces us to think of problems in smaller consumable chunks, as you never want to have a branch or deployment that has been under development for too long without merging into branch and ran in production

__Weekly Sprints__   

We need some "sign post" to tell us what we're shooting for.  This is the purpose of our weekly sprints.  The sprints aren't meant to be "release" points, but more a milestone target for us to hit.  These should be reasonable things we want to do and the Trello board should be broken up in these lists:

* Our Milestone - high level target we're shooting for
* Todo - items we need to do
* In Progress - what we're currently working on
* Completed - completed tasks, this could be made up of a few pull requests
* Business / Misc - items we need to work on from a business prospective
* Tabled - Things we need to do but are tabled for now, as we don't need to do it "right this minute".  However, it should be done within the next few sprints
* TBD - Items we haven't figured out yet, should be cleared as quickly as possible
* Retro (after the sprint is finished) - What we learned, what we want to run post-mortem on

__Hackathons__    

We hold two types of hackathons.  One is a "business related" hackathon, while another is a "random idea hackathon".  We try to hold hackathons every 4-5 sprints.  The "business related" is something that is related to our business, but may not be specific to the platform we're building.  For instance, 

###Trello Board Management

Here are some simple rules for our board management

* A board should be created for each sprint
* The board title should be clear and concise so anyone can figure out what you're trying to do
* When someone pulls something from todo -> in progress, they should assign themselves to the card.  Each person is responsible for assigning themselves tasks, but sometimes someone may assign a card to you
* Don't try to stuff too much, if there's over 20 todos, we might have over-stuffed it
* Things that don't get done, should be moved to the next sprint, or put in the ["Sprint Graveyard"](https://trello.com/b/QQc4J4RQ/sprint-graveyard).  The idea of the graveyard is to put items that don't make sense after we've gotten a bit into it or something we've tabled indefinitely.

__Sprint Completion__

* Move lists (Tabled, Fault Tolerance, Business/Misc) to the new Sprint cycle
* Change color of the previous sprint to "Gray"
* Go through In Progress list and move the ones that can not be finished, but the idea is things in "In Progress" shouldn't be left in there for a long time
* Look at Todos and either move it to Sprint Graveyard or to the next sprint
* Look at the latest sprint and make sure there's not too many "In progress" or "Todo" items
* Look at Milestones and determine if we've met them and any that haven't been met, should be moved to the next Sprint's milestone (unless it was deemed invalid)
* Complete a Retro for the finishing Sprint, and create necessary todos


### Useful Links

[Brightergy Trello](https://trello.com/brightergy2)    
[Hackathon](https://trello.com/b/cTP0Grnn/hackathon)    
