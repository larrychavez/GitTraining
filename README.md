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

Get the url for the repository you want to clone from GitHub:
https://github.com/DellGDC/GitTraining.git

Open Git Shell
Type the Git command to clone:
* git clone https://github.com/DellGDC/GitTraining.git

Saving changes to your repository (add and commit:
You must save changes to your local repository instance before pushing to GitHub.

First add the files to git that you want saved.
* git add .
(Yes, that's a period after "add", which means you want to add everything).

Second, commit the changes to your repository:
* git commit -a -m "a clear, concise message of what your committing"
the "-a" meands