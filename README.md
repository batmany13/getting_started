Welcome to Brightergy's R&D team, primarily responsible for building the Brighterlink Platform.  This is your one stop shop for getting to know our system, tools, processes and technology better.

## Development Methodology and Tools

We use a Continuous Delivery model here, with weekly "Milestone" sprints.  The idea here is, we have a weekly "goal" that we want to hit, but we're pushing code to production constantly, so if we need to fix bugs, or clean up something, we can do it without waiting for an official "release".

###Branching Strategy
Since we do Continous Delivery, we have to employ some specific techniques for our branching, here's a quick walkthrough

* Use master as the deployment / golden copy
* Branch off of master per Issue/Feature, make it as "atomic" as possible
* Make sure your branch test build passes
* Pull Request into Master
* One or more colleagues reviews your PR, makes comments
* The reviewer merges and deletes the branch
* Profit

__Things to avoid__  

* Keep it Atomic - You will probably see some minor fix while working on your code, but try your best not to fix it as part of your branch.  Unless it is specifically related, create a separate branch from master and do the fix there, trust me you'll thank us for it
* Branching off of a branch - always branch from master, don't do a branch of a branch
* Do not check in code without accompanying tests

__Things that don't need a branch__

* Simple README.md changes
* Cleaning up white space

### Our Tools
[GitHub](https://github.com/Brightergy) - Our code repo, DUH!   
[Semaphore](https://semaphoreci.com/) - Continuous Integration for testing our builds    
[GitHub Issues](https://github.com/Brightergy/brighterlink_io/issues) - We track our bugs here   
[Trello](https://trello.com/brightergy2) - Our sprint boards, we use this with GitHub Issues   
[Slack](https://brighterlink.slack.com) - This is our central communication tool   

__Relevant Links__     
[Dymitruk Model](http://dymitruk.com/blog/2012/02/05/branch-per-feature/)    
[Feature Branch Workflow](https://www.atlassian.com/git/tutorials/comparing-workflows/centralized-workflow)

## DevOps Culture

We have a deeply ingrained DevOps culture here, it doesn't mean you have to be an expert on everything, but it means you should care and value all the parts of delivery our product, from the code all the way to running in production and getting customer feedback.

[Heroku](https://dashboard.heroku.com/) - PaaS Provider, also use it for Continuous Delivery    
[PostgresSQL](https://postgres.heroku.com/databases/brighterlink-api-heroku-postgresql-cyan) - Database (Heroku Add-on)    
[Honeybadger](https://app.honeybadger.io/projects/47512/faults?q=-is%3Aresolved+-is%3Aignored) - For monitoring exceptions    
[Papertrail](https://papertrailapp.com/systems/brighterlink-api/events?r=656373878381432838-656393487524384768) - For log aggregation (Heroku Add-on)    
[Loader.io](https://addons-sso.heroku.com/apps/brighterlink-api/addons/f7604646-27e9-494f-86c9-396b823af81c) - Load testing

### Our Deployment Model

* Each branch gets built on Semaphore and tested
* Merge branch into master after a PR
* Heroku it is then "automatically" deployed into production

### Team Collaboration

We pretty much use slack for most of inter-team communications so you'll notice a couple of channels to be aware of

* [#devy](https://brighterlink.slack.com/archives/devy) - this is pretty much where all of our various tool communications go, so anything from CI to CD to Exceptions go here    
* [#critical](https://brighterlink.slack.com/archives/critical) - these are critical system alerts, and most likely a "system" down type scenario

## Architecture

We have two main components in our system, our "front end" and our "back end".  The front end is our user interface, and it connects to the backend via Websockets and REST apis.

[Brighterlink UI](https://github.com/Brightergy/control-ui) - Elixir / React / JS Frontend    
[Brighterlink API](https://github.com/Brightergy/brighterlink_io) - Elixir/Phoenix Backend    

### Third Party Tools

* [Auth0](https://manage.auth0.com/#/) - handles our user management    

### [TODO](todo.md)


## New Employee On-boarding Checklist

* Get access to GitHub    
* Get access to Slack     
* Give them this page     

### Wiki

The getting started information are available in the [Wiki](https://github.com/Brightergy/getting_started/wiki).
