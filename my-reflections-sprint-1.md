# My Reflections - Sprint One 

In addition to the challenge specific reflections, answer the following questions:

# Command Line Primer 

<!-- Copy the answers you wrote in your temporary file earlier, under the sections below -->

### In a couple of sentences, how would you describe the command line in plain English? Can you think of an analogy for it?
The command line is another way of navagating the files on your computer. Instead of using the GUI (Graphical user interace) to 
navigate/create/move files they are displayed in text format . And no i can't think of analogy! 


### Did you stick to the timebox guidelines? If not, what change would you make next time?
More or less, i went slighty overboard with some of the command line stuff, next time just stick to exactly what is described in the tasks and not try to get ahead of myself


### Name 5 commands you used, and what they do
ls   list all items in current directory
cd  		-(opens another directory) 	
Start 		-Opens file
mkdir		-creates folder	
Touch 		-creates file 


### Did you learn anything unexpected?
To be honest i didn't know what to expect! So everything is new, so.. i expected to learn new things and i did, so i guess nothing, 
but everything, unexpected. 




# Version Control with Git

<!-- Copy your reflection answers into this file -->

### Whats the difference between git and GitHub?
Git is a local programme for version control, while github is an online server where developers upload or 
        "push" different versions of files they might be working on individually or colabratively


### Can you think of an analogy to describe them?
As described in one of the videos and maybe websites pushing a version from git to github is like a save point of that version,
         like taking a photo of board game. The photo has a time stamp on it and info of where everything is at that time. A version is
        like that and allows reference and the ability to restore that version if needed. 



### Do you think you would still remember the difference a week from now if you didn't revisit the material?
   Abosolutely. 


### Did you stick to the timebox suggestions? If not, why not?

No, i went a bit far into commiting things to github as it was so fun and interseting...



# Install and Explore Git 

<!-- Copy your reflection answers into this file -->

### What is a GitHub work flow?
        GitHub work flow is a way for a group to colaborate on a project by using version control. Version control is a way to mitigate having a thousand different files of say a poem (e.g poem 1, poem 1 final, poem 1 real final). Instead Each version is a "snap shot" taken of it like taking a photo with a time and date on it, and who did the work. This way if you make a change you don't like you can go back The orignal version, or any other version that is in the respository either  on the remote server on git hub, or on a local computer using Git. Git uses branches to be able to work on files, without affecting the master copies.  These branches are like copies of the original, and can be worked on independetnly and localy without changing the master copy or the master branch. Each time a change is made, it can be commited to github, creating a version. These versions are tracked by Git so that all the changes that are commited are recorded. The changes made locally can also be uploaded or pushed to the remote server aka Github, for the team to reveiw, accept change or decline, then can be merged to the orginal copy. 


### What did you notice about your own learning? What did you do when you were confused or blocked?
        It has been good to activate my brain again! when i've felt confused with infomation overload, or a concept i can't get my around somtimes i will have a 5 minute break and come back to it and just read slowly, and keep going hoping it will make sense with an activity or further on in the material. If it doesn't i leave it , and come back to it later. I find as i bring more pieces of information together the bigger picture becomes more clear, and the little bits of information seem to fit better in my rbain. 


### Is there anything you'd do differently if you were to repeat the learning exploration again?
        No i don't think so, i feel i went through the course step by step and it was fine. 



# Track and Commit Primer!

<!-- Copy your reflection answer into this file -->

### How would you describe stage and commit to your non-tech-savvy friend?  

   If the command line is like a catupult, staging would be loading the stone into the catupult and commiting would be firing it. The two stages are loading and firing, 
        like staging and commiting. In staging things are loaded to be ready to be commit. This could be muiltple files from jpg or html etc, and commiting is then like saving
        or taking a picture of only the loaded files. 



# Branch, Pull, Merge

<!-- Copy your reflection answers into this file -->

### What is Master?
 Master is the main trunkline or published version of a remote branch. Master in a local branch is the same, which then can be branched off to work on edits without
        affecting the master, then after edits are made can be merged together with the master by the git merge command. If you want to work on something in a team that you 
        need changed on a remote master branch but you don't have access to it, you can fork the entire repository, then clone it down to a local with git clone "url".
        From there you would want to create a branch with command "git checkout -b (new name)" . Then create or edit the file you want to change, you will want to
        add the file with git add, then git commit,  afterward, switch back to the master with "git checkout master", then "git merge (new name)" this will merge the two 
        branches together with your new change. Afterward you can use "git push origin (new name)" which will create a pull request on the original web page ( i think)



### Why create a Branch?
as explained above 


### Do the concepts introduced feel intuitive or difficult to understand?

For some reason the concept of branches seems intuitive since we all know about trees. And i guess watching enough movies with alternative timelines as helped me 
        to undesrtand the difference between "entangled" items where if you changed one it automatically affects the other, and "individual" items, where they are 
        indivuals until brought together. This has helped me understand the difference between local, remote, master and alternate branches. 



# GitHub Fork & Clone

<!-- Answer the following questions -->

### What are some examples of when you would fork? 
        If you are working on a shared public project but don't have access to edit/clone the official repository you can fork the whole prjoect to the developers server side repository.  The developer can then clone their own copy, work on it and push it to their server side, which afterward a pull request can be made to merge the branch the developer has worked on into the official repo. 


### Write your own step-by-step fork and clone instructions. Describe what you did.
        On github, 
        Go to server you want to fork, at the top right there will be a fork icon. Click it and choose the account you want to fork it too. Aferward this will create a fork in that account.

        Go to that account and copy the clone url, then in the Git Bash command line, use Git clone "url" to clone the repository to the local pc (make sure you clone it into a desired directory, use pwd command to print wokring directory to check)

        This will haved created a clone in whatever directory you were in when you typed it. After this it is reccomended you create a another branch to then work on any changes. Create a branch using command git checkout -m name (where name is the name of branch) . You can then begin to work on this branch without affecting the master branch .

        The reason for this If for some reason, while you are working on the clone, the upstream master branch is changed, you can simply sync your master without affecting any changes to you work since yuo are working on a seperate branch. Use git pull upstream master to do this. Then when you come to merge your branch to the master it will be the same master as the orignal. 

        when you are finished and what to create a pull request back to the original server, obviously use the correct line to bring the information back. From the secondary branch, git add (files you work on) git commit -m "commit message" then switch to the master line with git checkout "name" . Then use git merge "name" to merge the two branches. After that, git add branchname git commit branch name git push origin . 

        From there the files should appear on Github, which you can then select an option to create a pull request back to the orginial server. 


### Did you have any moments where it all clicked? What clicked?
        Not really, i felt like it all progressively built. Actually from the onset, watching the into video by Joseph, i actually followed along in another window copying him. Having copied him and then going through reading the rest of the matarials and practising just sort of made aware of what was going on in the orignal video. 




# Setup Repo & Create Blog

### Reflect on this activity. When did you feel frustrated?
        Not even once, it was the easiest activity so far. 


### If you didn't already know that this is the way websites are made; was it what you pictured? How does the reality of this process differ from your preconceptions?

        I guess i didn't really know. I did think people would use a programme like this to write code, but had no idea of the way it was all intergrated. So i've always been curious, and this has been an awesome learning experience, i have loved learning about the command line. 



# Thinking like a programmer

### Describe the process for solving problems



### Will you follow that process? How?



### What did you learn about flipped classroom?





# Introduce yourself

### What was it like trying to summarise yourself to a group of strangers? 



### Could you feel your ego? Were you self conscious? 

