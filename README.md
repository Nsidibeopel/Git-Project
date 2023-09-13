# GIT-PROJECT

Initializing a Git Repository

To initialize a git repository, I used the commands below:

Step 1. Create a directory using the command: mkdir JoanDevOps-Project'

Step 2. Change to the directory created using the command: cd JoanDevOps-Project\

Step 3. While inside the folder, run the command 'git init' to initialize the repo

Please take a look at the screenshot below.

![Capture](https://github.com/Nsidibeopel/Git-Project/assets/143354400/a09cb4ab-d014-411e-8d03-b9213c8cf518)

Making a Commit

To commit is to save changes, for example, adding, modifying or deleting a file. 

When the command is run, it takes a snapshot of the current state of the repository and saves it to the .git folder inside the working directory.

Here are the steps to make a commit on Git

Step 1. Create a file named idex.txt

Step 2. Add a text "My First Git Commit" to the file created using the following command

echo "My First Git Commit" > index.txt

Step 3. Use the command 'git add .' to update or add the changes to the repository.

Step 4. Finally, commit the changes to git, run the command git commit -m "First Commit"

Please take a look at the screenshot below.

![commit](https://github.com/Nsidibeopel/Git-Project/assets/143354400/ef81ee17-e2e0-4f7e-9fb8-1cc5c571deb2)

WORKING WITH BRANCHES

Git branches help create a different copy of of your source code. Changes made to the branch do not affect the Main copy.

The Git branch is especially useful when adding or developing new features to an application.

The Git branch also helps with collaboration within remote teams. 

They can create separate branches while working on the same feature at the end, they converge their code into one branch.

To create a branch, I used the command git checkout -b my-first-branch

To see the branches on the local git repository, I used the command git branch

To change into the previous branch or main branch, I used the command git checkout main

Please see the screenshot below

![Branches](https://github.com/Nsidibeopel/Git-Project/assets/143354400/8060339b-baf8-4b2d-b984-cab347a74aae)

MERGING BRANCHES

Git makes it possible to merge the content of a branch to another branch. To practice this, I created and switched to a new branch using the command below

git checkout -b my-second-branch

I created a text file named trial.txt using the command touch trial.txt

Next, I add a text to the file using the command echo "lessons on merging branches" > trial.txt 

I tried to run the merge command at this point but got a message 'already up to date'. I realised I had not committed the changes yet(see screenshot)

Next, I run the command git add . and then run the command git commit -m "my first branch commit" This saves the changes made to the file inside the branch

I then run the merge command after switching to the first branch using the command 'git merge my-second-branch'  See the screenshot below

![Merging branches](https://github.com/Nsidibeopel/Git-Project/assets/143354400/d3d20152-94af-4546-8c5f-11440b60409d)

To delete a branch, simply run the command git -d my-second-branch. See screenshot below

![delete branch](https://github.com/Nsidibeopel/Git-Project/assets/143354400/56eeea96-9d07-4d4d-ae1a-6cd152da49ec)


COLLABORATION AND REMOTE REPOSITORIES

Git is a distributed version control system which enables the sharing of source code and tracking changes made to source code. This can be achieved by 

creating a git repository, initializing it, committing any changes made, and even creating branches. Github, on the other hand, is a web-based platform.

Repositories created on git are hosted on GitHub such that they become accessible over the internet, which fosters collaboration because remote teams can now view, update and

make changes to the same repositories.

To remotely host the local git repository on GitHub, you need to create an account on GitHub. After creating an account successfully, I push my local Git repository to my GitHub

By taking the following steps

Step 1. Create a new repository on GitHub named RemoteGitHub-Practice. See the screenshot below

![GitHub Repo Created](https://github.com/Nsidibeopel/Git-Project/assets/143354400/9844e9ef-6135-43bb-a2ca-42c9acd68bd5)


Step 2. Copy the remote link on the new GitHub repo created and paste it into the git bash terminal along with the command below

        git remote add first-remote-repo https://github.com/Nsidibeopel/RemoteGitHub-Practice.git

Step 3. Commit the changes by running the command below

    git commit -m "first-remote-commit" See the screenshot below for steps 2 and 3

   ![commit repo](https://github.com/Nsidibeopel/Git-Project/assets/143354400/4f98538a-4872-4467-88e0-877c160560ce)
        
        

Step 4. After committing the changes to push to the remote repo on GitHub, I used the command below

       git push (which gave me an error message with the correct command to use) See the screenshot below

  ![push command](https://github.com/Nsidibeopel/Git-Project/assets/143354400/20e2af54-df75-485e-b71c-3449db8ccb31)

CLONING REMOTE GIT REPOSITORY

The clone command is a tool for downloading a repository into a local machine. 

This tool is important because it helps team members to be able to work on a remote repository on GitHub, 

It is best practice to make a copy of the remote repository on their local machine and create a branch where modifications can be made.

To get a local copy of the remote repository, run the clone command below

git clone https://github.com/Nsidibeopel/RemoteGitHub-Practice.git See screenshot below

![clone command](https://github.com/Nsidibeopel/Git-Project/assets/143354400/9338a354-3b72-4afb-b2c7-21415d2e19fb)


