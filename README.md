##Assignment 1: Git Usage

In this assignment, you will get familiar with Git and some of its main features. The assignment assumes that you are working from the command line, and we will simulate the presence of multiple users by using two terminal windows. If you are already familiar with Git and a specific Git client, feel free to use that, as long as you do what the assignment requires.

In the following, the term “REPO” is used to indicate the repository created for your assignment. You will receive an email at your your VCU email address with an invitation to the join the cmsc355-vcu organization on GitHub. After you accept the invitation, you will be able to see REPO in the list of repositories on your GitHub account by switching to organization cmsc355-vcu.

Please also make sure to read the whole assignment before getting started and to follow the instructions to the letter (e.g., use the exact commit messages provided in the assignment, rather than variations of them). If you don’t know how to accomplish a task, either consult Git’s help by running “git --help [command]” or leverage online resources. If you receive an error while executing a Git command, make sure to read the error message, as Git often suggests exactly the right thing to do.

I also suggest that you use GitHub's "Network" view to monitor the state of your local and remote repository throughout the assignment. To do so, go to the GitHub page for REPO, select menu "Graphs" on the right, and then select the "Network" tab at the top. In this way, you will have a visual representation of how the repository evolves, which can be very useful for better understanding Git and how it operates. 

Finally, I suggest that you practice the assignment on a separate repository and then perform the assignment on REPO when you feel comfortable with the various commands. 
  
###Assignment Instructions
####Part 1 (Terminal 1)
Before you start, make sure to specify your name and email address using command “git config”, if you haven’t already.

1. Open a terminal window
2. Create and go to directory Student1
3.	Clone REPO
4.	This should create a directory called assignment1-user (user will be replaced with your own eID) under directory Student1
5.	Go to directory assignment1-user (here you can open the Network view in GitHub and start monitoring how your repository evolves)
6.	Make sure that the directory contains a file called MyPrivateRepo
7.	Create and go to directory Part1 (under assignment1-user)
8.	Create a file called myinfo.txt that contains only one line with your first and last name
9.	Commit the file to your local repo with comment “Added myinfo file”
10.	Create a branch called “development” and switch to it
11.	Create a file called dev1.txt (the content of the file is irrelevant)
12.	Commit the file to your local repo (it should be in branch “development”) with comment “Added dev1 file”
13.	Switch to the “master” branch
14.	Edit file myinfo.txt and add your zip code in a separate line (feel free to make up the code, if you don't want to use yours)
15.	Commit the file to your local repo with comment “Edited myinfo file”
16.	Merge the “development” branch into the “master” branch (any commit message is fine here)
17.	Push all branches to the remote repository

####Part 2 (Terminal 2)
1.	Open a second terminal window
2.	Create and go to directory Student2
3.	Clone REPO
4.	Just like before, this should create a directory called assignment1-user under directory Student2
5.	Go to directory assignment1-user/Part1
6.	Create and switch to the “development” branch
7.	Create a file called dev2.txt (the content of the file is irrelevant)
8.	Commit the file to your local repo (it should be in branch “development”) with comment “Added dev2 file”
9.	Create a branch called “temp” and switch to it
10.	Create a file called mytemp.txt (the content of the file is irrelevant)
11.	Commit the file to your local repo (it should be in branch “temp”) with comment “Added mytemp file”
12.	Create and commit to branch “development”, with the usual comment, a file called dev3.txt (the content of the file is irrelevant)
13.	Merge the “temp” branch into the “development” branch (any commit message is fine here)
14.	Merge the “development” branch into the “master” branch (any commit message is fine here)
15.	In the master branch, edit file myinfo.txt and add your eID in a separate line
16.	Commit the file to your local repo with comment “Edited myinfo file again”
17.	Push all branches to the remote repository

####Part 3 (Terminal 1)
1.	Go back to the first terminal
2.	Make sure to be in branch “master”
3.	Edit file myinfo.txt and add your phone number in a separate line (feel free to use a fake phone number)
4.	Commit the file to your local repo with comment “Edited myinfo file for the third time”
5.	Push the master to the remote repository. To do so, you will have to suitably pull changes from the remote repository and handle conflicts. In handling conflicts, make sure not to lose any content, not to have any of the extra text added by Git to mark the conflicting parts, and to preserve the order of the information as it appears in the assignment. (Any commit message is fine for the merged file(s).)
6.	Tag the current version of the master as “Version1” and push the tag to the remote repository.

At this point you are done, and your remote repository should look like the one in the figure below in the "Network" view on GitHub. If it doesn’t, it means that you made a mistake in one of the steps. Given the fact that this assignment is fairly simple, as it mainly consists of executing the provided steps, I expect the network view to match the figure below exactly and will deduct points if this is not the case. Similarly, I expect all the commit messages and the content of the files in the repo to be correct.
<img  alt="part3" src="https://cloud.githubusercontent.com/assets/1023063/22374035/5dada8ee-e472-11e6-8b2b-905295236771.png">
To submit your assignment, post in Blackboard a link to the URL of your private repository.
