####Outline of Pull-Request workflow process:

1.	Fork Main Repo
2.	Clone User Repo 
3.	Create a branch when working on feature changes
4.	Fetch and merge Changes from upstream
5.	Merge Feature branch with local master
6.	Push local Master to User Repo
7.	Initiate a Pull Request from User Repo
8.	Merge Pull Request on the Main Repo 

Note: Steps 1 and 2 are done once.  Most development will be a cycle of steps 3-8

####One time activities In Pull-Request workflow process:

**Fork Main Repo:**  This is done on github.com.  When signed in as yourself, you then navigate to the appropriate repo, click on fork.  A copy of the repo will now be in your account.  

**Clone Repo:**  This will bring your copy of the repo down to your machine.

	git clone https://github.com/[your github username]/WeAreCohort.git.

**Create Upstream Fetch:**  This allows you to get updates from the Main Repo.  This way you can get the updates that have been put in the main repo.

	git remote add upstream https://github.com/TechTank-DataScience/WeAreCohort.git


####Common Commands During Feature Creation

**Create a Feature Branch (Optional – default branch is master, which is fine to develop on):** This creates a branch from your currently checked out branch
	git checkout -b feature1

**Fetch changes from Main Repo (upstream):** This gets the changes and puts it on your local machine in a branch called upstream/master

	git fetch upstream

**Merge changes from one branch to another:** This merges changes from one branch with another branch.  The example merges changes from the Main Repo with the feature1 branch
	git checkout feature1
	git merge upstream/master

**Push Changes From Local Machine To User Repo:**  This is done after a feature has been completed and merged into the local master branch.  This will then put those changes into the User Repo on GitHub
	
	git push origin 

**Initiate Pull Request:**  This is the process by which changes are applied to the main repo.  The basic idea of this is that the User Repo is asking the Main repo to take the changes in the User Repo and merge them with the Main Repo.  All of this occurs on github.com

1.	go to your User Repo on github.com
2.	on the right hand side click pull requests
3.	click create new pull request
4.	Add comments and create the new pull requests

**Merge Pull Request on the Main Repo:**  This is the final step for putting changes into the main Repo.  If possible, the person accepting the merge request on the main repo should not be the person who is making the pull request.  This way all of the code will have a chance of getting reviewed before being committed to the main repo.
1.	go to the Main Repo on github
2.	click pull requests
3.	if the changes look good go merge and close the commit


 
**Graphical outline of common workflow:**




Useful links:

[http://git-scm.com/book] - great resource if you are new to git.  Helps with basic understanding of git

[https://help.github.com/] - specific to github operations, but there is a lot of basic git operations explained

[https://www.atlassian.com/git/tutorials/comparing-workflows/] for different ways of going git workflows.

