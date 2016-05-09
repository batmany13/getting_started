### Our Deployment Model

We are experimenting with Heroku Pipelines for our deployment model.  Pipelines only have 3 stages, "review -> stage -> prod".  This is the model we are using

* Each branch gets tested on Semaphore app
* Pull request is created, a review app is available but not automatically created
* Merge the branch into master after a PR
* Semaphore runs again
* Stage gets automatically deployed with the changes
* Any additional testing can be done
* Promote the change from stage->prod, be sure to review the changes

### Post mortem analysis

A key concept to continuous delivery is to have a "continuous improvement" model, which means we have to have good and productive post mortem analysis for any issues we've run into.  This ensures that the system is always kept fresh and up to date, and we don't take reactionary precautions (ie end continuous delivery) whenver there's a production issue.

* __No blame culture__ - if any issue arises, we attack the issue, not the person.  Most of the time, it is not the person that failed the system, but the system that failed the person.  In any post mortem, we have to address the root cause
* __5 Whys__ - This comes from lean startup, but you ask "why" 5 times, to really get down to the root cause.  The concept here is, we should be fixing the root cause, not the symptoms.
* __Patch forward, no reverting__ - This comes from FB, where we should be thinking about patching by fixing the bug, not reverting the code.  It's a slight shift in mindset, but if We are delivering micro-chunks of functionality, it should be much easier to patch specific points.  It can be daunting when you are delivering 1000s of lines of changes, but this wouldn't be our case.
* __All issues can be reviewed__ - this doesn't have to be a product or software issue.  It could be a process or tools or communication issue we want to improve.  We may find that through our "5 Whys" that some of the improvements we need to make is more training or process, so we should be open to all improvements.

### Team Collaboration

We use slack for most of our inter-team communications.  There are a few channels to be aware of from a DevOps standpoint

* [#devy](https://brighterlink.slack.com/archives/devy) - this is pretty much where all of our various tool communications go, so anything from CI to CD to Exceptions go here    
* [#critical](https://brighterlink.slack.com/archives/critical) - these are critical system alerts, and most likely a "system" down type scenario
* [#general](https://brighterlink.slack.com/archives/general) - Pull Requests comes to general, so it won't get "lost" in the various notification channels.
* [#support](https://brighterlink.slack.com/archives/support) - Customer and prospective client communications go here.  Internal support may go here as well


###Useful Links

[Etsy Deployment Model](http://www.infoq.com/news/2014/03/etsy-deploy-50-times-a-day)
