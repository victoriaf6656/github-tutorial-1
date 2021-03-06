# GitHub Tutorial

_by Bali DeFreitas/Deadbeat_

---
## Git vs. GitHub

Git, the code we use within terms of planning and forming ideas. Git is the base of the coding used via Github, this means that Git can't exist without Github. However Github can exist without Git as Github is a cloud system. A cloud system is a form of storage and it's used to hold information online. This means that Github can store code from Git and even other websites (Example: Cloud9)  
  
Examples of using Git would be a piece of code referred to as ``git init``. This example will be explained better in ***Initial Setup***.

---
## Initial Setup

So you made it this far? Not bad, but things are probably gonna get more complex from here on out. When Initializing, you need a directory to work in ( Usually ``~/workspace``) and to initialize a directory, you would use this little piece of code titled ``git init``. Now I bet you're thinking, can't I just use it without the space in the middle. The answer is no, that space is required to actually have the code function. Let's dive into the basics shall we? 

### Codes  

``git init`` - When you start up the system, you can either cd (Check the code snippet cd for more info) into your directory. This code is used to give the directory the function of master, which is basically empowering it. When you used ``git init`` the directory should say ``~/workspace/directory_name (master)``. This means the code worked and you want to make sure you intialized the right directory because there is a git init. 

``cd`` - This is one of the more simplier pieces of code, it simply enters the directory. It's used often after creating a directory for the first time and often used to avoid initializing the wrong directory. This also means you should remember to do this piece of code to prevent any accidents. Basically make it a habit and never forget it.  

``touch`` - So you're inside the directory and now you wanna write something, maybe a love letter? Well I'm sure you're thinking "Time to use git file or git create." Well hold your horses, because the actual command is ``touch``. When you use this piece of code, it won't say it worked or not. It'll simply create the file and the bash section will move to a new line.

``mkdir`` - Now before you go off and try to make a directory with touch, just stop.``mkdir`` is short for "make directory." Directories are like folders on a computer. Directories hold files that are made inside of it. Now what if you accidently make a file and need to delete it you ask? Well that's the next code snippet in this long list of codes.

``rm`` - Remove or ``rm`` is made to delete a file that you don't want anymore. It doesn't ask to make sure to delete it. It'll simply remove the file and erase all your hard work, so don't go messing around with this piece of code because their isn't an undo command or something. But what if, you wanna delete the whole directory? Well it must be your lucky day because there is a piece of code for that too!

``rm -rf`` - This code is a even more deadly compared to it's little brother, it removes the directory and whatever is inside of it. However the one flaw of this code is that if you are inside said directory, it can not be deleted until you leave it and reuse the code! So if you are 100% sure that you wanna get rid of a folder and whatever is inisde of it, then shoot for the stars and use this code.

``c9`` - This is the last piece of code you'll need to know for initail step up. This code is quite the simpliest code ever made. t opens up a file from the `bash` command line. Now let's get more serious and dive into making a Repository.

---
## Repository Setup

So you and little Johnny wanna work on this magic project from different locations? Well that's what a repository is for! You can work together and create something magical via the power of repositories or repo for short. However it does have a lot of steps before you and Freddy can actually work on this project from afar. So let's begin shall we?

### _``Codes``_ 

Alright so you wanna make a repo, you're all _gitty_ and excited for this magical trip. First step to getting your repo is having a directory and some files in it. Second step is having a Github account (If you don't have one, please make one right now.) and going to "+" icon in the top hand right corner. See where it says "New Repository"? Click on it and read closely from here on out. Once you clicked it, it should take you to a different page that'll ask for the repository name. Insure that the name matches exactly with the directory name, otherwise you and Pedro are gonna have to make a new repository... or will you? We'll talk about that later for now, name it directly after the directory. You did it? Great! Now you have to link the Repo and the Directory with each other or for short term, make a bridge between the two of them. The repo will recommend that the directory/repo have a README of sorts, I suggest the same as it's the means of informing the readers and yourself of what the purpose of the repo.

So you made a repo? Grand, now you should go to your profile icon and click on the settings Once you're inside, enter the SSH and GPG, select SSH (This is to prevent the constant need for a password and stuff.) (Insure that you aren't a workspace) Title this SSH Key a cloud9 and copy and paste the second key. Now you open up c9 and open the Cog icon (Gear Icon) and open the SSH key section and paste the second key into the private section of the page. Now add the SSH key and go enter your workspace, ensure that you are typing in the ``bash`` section and type ``ssh -T git@github.com``.  
It should read "Hi _``username``_, you've success connected Cloud9 to Github!"  

Alrighty, you can now link your repository and local systems together and to do that magic, you need the SSH Key from the repo. You copied the link? Great, now type in _``bash``_ ``git remote add origin URL``. The url is just what you copied so place that inside the code where it says URL and check using ``git remote -v``.


---
## Workflow & Commands
Here is where all the other pieces of code that you can use.

* ``git init`` - Initializes the directory
* ``rm -rf directory_name`` - Removes a directory and if inisde uninitializes it
* ``git add file_name`` - This adds a file to the scene for commiting it
* ``git add .`` - This adds files
* ``git add --add`` - This adds all files to scene even those you have deleted
* ``git commit -m "message"`` - This commits it and saves all changes made to the file
* ``git remote add origin URL`` - Code used when linking a repository and local system together
* ``git push -u origin master`` - When pushing to the repository, we use this as a means of giving it a nickname for later usage
* ``git push`` - This pushes the file changes to the repository after using the origin master version
* ``git diff`` - This shows all the changes you made since the last commit 
* ``git log`` - This allows you to view the changes and commands you have done
* ``q`` - Just press that key when you wanna back out of Git log
* ``git checkout -- file`` - This removes a new commit and reverts a file back to it's previous commit.
* ``git rest HEAD file`` - Unstages a file and keeps the changes and reverts it back to it previous state
* ``git remote -v`` - Checks if you have a repo linked to the directory
* ``git status`` - It shows if you added a file and if you commited it, with Red being it not being added and Green being it hadn't been commit.
* ``git pull`` - Pulls back a previous commit from before
* ``git soft/hard HEAD rest^`` -  Soft removes the file from the commit, but keeps the add ons before hand.  Hard resets the file and deletes any commits and changes you made so be careful.




---
## Rolling Back Changes