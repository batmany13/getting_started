## Branching Strategy

Since we do Continous Delivery, we have to employ some specific techniques for our branching, here's a quick walkthrough

* Use master as the deployment / golden copy
* Branch off of master per Issue/Feature, make it as "atomic" as possible
* Use human readable branch names, but avoid super long names
* Make sure your branch test build passes
* Pull Request into Master
* One or more colleagues reviews your PR, makes comments
* If there are changes, the committer should comment to say "I am accepting xxx comments"
* The reviewer merges and deletes the branch
* Profit

__Things to avoid__  

* Keep it Atomic - You will probably see some minor fix while working on your code, but try your best not to fix it as part of your branch.  Unless it is specifically related, create a separate branch from master and do the fix there, trust me you'll thank us for it
* Branching off of a branch - always branch from master, don't do a branch of a branch
* Do not check in code without accompanying tests
* Making changes outside of the Brightergy workspace.  You might feel the need to try some stuff on your personal github and then migrate it, but try to avoid this.  Even if its some test code, you can manage it [here](https://github.com/Brightergy/hackr)

__Things that don't need a branch__

* Simple README.md changes
* Cleaning up white space

__Relevant Links__     
[Dymitruk Model](http://dymitruk.com/blog/2012/02/05/branch-per-feature/)    
[Feature Branch Workflow](https://www.atlassian.com/git/tutorials/comparing-workflows/centralized-workflow)
