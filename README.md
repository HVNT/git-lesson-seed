# Let's learn git!  

### Why should you take this course?
Ok, so you've finished your first Computer Science class at Georgia Tech. You understand how to write a simple program, compile it, and then run it. Congradulations, you're a coder. Things are about to get interesting for you. Now that you understand can write some code that actually does some thing it's time to take it to the next level, working on a team. Working on a team introduces new challenges. The biggest challenge your team will face will probably be not implementing the code itself, but how to implement the code in a distributed manner where everyone is contributing to one central project. This course will teach you just that: how to contribute your code in a organized scalable manner to a team project.

### What is version control?
Version Control is a system that records changes to a file or set of files over time so that you can recall specific versions later. Think a really lightweight "OS X" bootcamp for your CS projects. It allows you to revert files back to a previous state, revert the entire project back toa  previous state, compare changes over time, see who last modified something that might be causing a problem, who introduced an issue and when, and much more.   
source: https://git-scm.com/book/en/v2/Getting-Started-About-Version-Control

### What is git?
Git is a Version Control System. There are many Version Control Systems out there, git is just one of them. We are teaching git because we feel like it has been accepted by the software community as the best practice Version Control System. Lately, we've even seen recruiters talk as if it's a requirement to any Computer Science graduate's resume.

### What is GitHub?
Git is great, but we need a put our project that everyone can access: AKA the internet. There are a lot of great services out there that provide this ability. For this course, we will use GitHub. We chose GitHub because, like git, we feel like it has been accepted by the software community as the best practice hosting site for projects under git Version Control.

### Ok now that we are through all of that, lets finally get our hands dirty and beafin' up that resume.  

### Step 1: Installing git. 
To get started, we need to make sure you have git installed on your Operating System. If already have git installed you can skip this step and continue to Step 2.  
Go to https://git-scm.com/downloads and download the appropriate git for your Operating System.  
Once you have the .img or .exe (OS X or Windows, respectively), go ahead and click the file to run it. Follow the instructions and install git.  
You can confirm you have git by opening up your terminal (or window prompt) and entering the command 'git help'.  
Once you have confirmed git is installed continue to Step 2.

### Step 2: Getting started.
The command 'git help' you ran in Step 1 ran the 'help' function in git using gits command-line interface (CLI). A CLI is simply a text based interface that you most commonly interact with through your command line (i.e. your terminal or window prompt). A CLI is just a way to interact with an underlying program, the same way your clicking the 'refresh' button on your browser interacts with it's underlying program. An interface of any time is simply a means for a program to digest user input. You can now continue to Step 3.

### Step 3: Making your first git project.
Now that you know what git is and how to interface with it via the command line, lets make your first git repository.  
Go ahead and make a new folder wherever you'd like (your desktop might be easiest, but it doesn't matter) and open your command prompt and navigate to it (using the command cd). Once you are in the folder inside your command prompt, go ahead and make your first git repository using the command 'git init'. There should now be a .git directory in the folder you created if you followed the steps correctly. If this is the case, continue to Step 4. 

### Step 4: Making your first GitHub repository.
Navigate to GitHub.com; create an account if you don't already have one. Create your first GitHub repository and name it whatever you'd like. Once you have a repository set up continue to Step 5.

### Step 5: Making your first git commit.
Now that you have a GitHub repository, lets point the git project you made in Step 3 to the GitHub repository you made in Step 4. Navigate back your project from your command line. To point your git project to your GitHub repository enter the command 'git remote add origin git@github.com:YOUR_REPO_NAME_HERE.git'. Replace "YOU_REPO_NAME_HERE" with the name of your GitHub repository. You can check if this worked by typing 'git remote -v'. You should see two lines, both the same https url, with one saying "(fetch)" and another "push". Your terminal should look something like this (ignore the stuff to the left of the hunt% and look at the response on the two lines after the command git remote -v is invoked).  
![alt text](http://i.imgur.com/mZP3dYs.png "Confirmation for step 5.")  
If you see the same two lines after 'git remote -v' continue to Step 6.

### Step 6: Pushing your first commit to GitHub.
Ok, lets get some stuff on your GitHub project finally. In same directory as this README.md file, there is an "index.html" file. Copy and paste that file into the git project you made in Step 3. Once the "index.html" file is in that project, go back to your command line and navigate back to it. Right now we have our "index.html" file in the same folder as our git repository, but it has not been added it. Lets do that. Go ahead and type in the command 'git add -A'. The git "add" command takes uncommitted changes from the files in your local git repository and stages them in git committed. Next, type in the command 'git commit -m "my first commit"'.
The git "commit" command takes your local git changes that are currently staged and pushes them to branch your active local origin branch. This is great! Currently, we have our "index.html" file under version control! We can confidently make any changes we'd like now to the index.html file with the knowledge that we can revert it back to any previous moment in time (as long as we committed it at that moment, which is why you should commit often!). It's awesome that we have it under version control locally, but this is a group project and other people need it too! To make that possible we need to push our committed changes up to GitHub (origin). Do this by entering the command "git push origin master". The git "push" command push changes to the specified location. In thise, that location is "origin master". "Origin" is telling git that we are trying to push our committed changes to somewhere outside of this computer; in this case, "origin" is whatever yous et it to in Step 5. "Master" is telling us we want to push these commits to the master branch on "origin".

### Step 7: Making your first branch.
You're getting the hang of this, good stuff! In the last step we pushed our committed code up to the master branch on our GitHub repository. This is fine when you are hacking together a quick project that only you are working on, but is a huge no-no when working on team projects (which you are right now). When everyone is just pushing their commits up to master merge conflicts are going to happen, its inevitable. Also, commits will overwrite eachother and code will be lost. You will easily destroy the purpose of Version Control uninentionally. We avoid merge conflicts, and keeping everyone on the team in sync, by using a git feature called branching. Branching allows us to essential copy the entire repo in an isolated environment, implement in a safe envormnet, commit changes in their, testing etc all while staying in sync with the master branch. This allows big features to be developed in isolation where we know they can not break anything. Once the feature is stable and testing, we will put the branch's code into master.

### Step 8: Making a change on your branch.

### Step 9: Pushing your branch to your GitHub repository

### Step 10: Making your first pull request and merging it into master.

### Step 11: Synchronizing your local git repository to origin master.

### Step 12: Lets see if you can do it on your own. (Repeating steps 7-11).

