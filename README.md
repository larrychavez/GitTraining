Git training repository.

Use this repository to practice using git without the fear of breaking anything.

This repository is public, so please do not add private or confidential information.

Documentation:
http://git-scm.com/book

Concept:
http://git-scm.com/book/en/Getting-Started-About-Version-Control#Distributed-Version-Control-Systems

Git is a Distributed version control system. This means instead of having a central location from which everyone works on directly (like a shared server), every person has a complete copy of the repository stored locally on their computer. Git, then, helps everyone keep their work in sync through merging and version control. Clients (you) don’t just check out the latest snapshot of the files: they fully mirror the repository. Thus if any server dies, and these systems were collaborating via it, any of the client repositories can be copied back up to the server to restore it. Every checkout is really a full backup of all the data.

Furthermore, Git deals pretty well with having several remote repositories it can work with, so you can collaborate with different groups of people in different ways simultaneously within the same project. This allows you to set up several types of workflows that aren’t possible in centralized systems (shared folder), such as hierarchical models.

Cloning a git repository:
http://git-scm.com/book/en/Git-Basics-Getting-a-Git-Repository#Cloning-an-Existing-Repository

==========================================================


Open Git Shell
Type the Git command to clone:
* git clone https://github.com/DellGDC/GitTraining.git

==========================================================

Navigating folders with the command line:
"cd" - means change directory;

* cd folderName
navigates you into the folder folderName.

* cd ../
navigates you to the parent folder.
* cd ../../
navigates you to the parent folder two levels up

you can combine these commands.... say your in another folder named otherFolder which is on the same level as folderName. To get to folderName in one command:
* cd ../folderName

To list folders:
* ls

Now... navigate to the GitTraining folder to start your training.

==========================================================

Saving changes to your repository (git add and git commit):
http://git-scm.com/book/en/Git-Basics-Recording-Changes-to-the-Repository#Committing-Your-Changes

You must save changes to your local repository instance before pushing to GitHub.

First add the files to git that you want saved.
* git add .
(Yes, that's a period after "add", which means you want to add everything).

Second, commit the changes to your repository:
* git commit -a -m "Add a clear, concise message of what your committing inside these quotes."

==========================================================

Pulling changes from GitHub (git pull):
http://git-scm.com/docs/git-pull

AFTER you commit your changes, git pull command.
* git pull

==========================================================

Pushing to GitHub: (git push)
http://git-scm.com/book/en/Git-Basics-Working-with-Remotes#Pushing-to-Your-Remotes

if pushing to the master branch, after committing your changes:
* git push -u origin master

If pushing to another branch
* git push -u origin branchName


==========================================================

Workflow:

To avoid the most conflicts or issues, you should subscribe to this workflow submitting changes to GitHub

In yor local repository, make sure your in the branch which you need to do your work:
* git status

To push changes, do these tasks in this specific order.

* git add .
* git commit -a -m "a great message"
* git pull
* git push -u origin branchName

Git automatically attempts to merge changes from the server, but it cannot do this unless you have your changes committed. Nor can it merge your changes on the server. So for the least amount of issues, you mush commit your changes, pull the server changes (which will to an automatic merge), then push your changes.