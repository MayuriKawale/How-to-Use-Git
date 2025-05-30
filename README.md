This repository is made for people who are getting started to use Git

# Creating a Local Repository:
By default, there is a single branch named `master`. Every other branch is like a independent development on the `master` branch.
1) Make a new directory
   Create a directory which will be your local repository
   ```
   mkdir myGitProject
   ``` 
2) Initialize a repository
   To initialize this directory and make it your local git repository, run the following command within the directory
   ```
   cd myGitProject
   git init
   ```
   When you initialize, then you should see the following in your local repository
   
   ![image](https://github.com/user-attachments/assets/f2e5c26f-f4a3-4410-9e8a-99b81fa03e7e)

# Commit to the local repository:
1) Check the status of files in the working tree and staging area, use `git status`
   Since there is nothing in this repository, we should see the following message :
   
   ![image](https://github.com/user-attachments/assets/fe02b53d-7864-4fca-a90c-cbe599ced57f)

   If you initialize a directory with some content already, you should still see a message about untracked files as you need to first add the files from this directory for tracking using git version control.
   Generate a text file using `touch` and then check the status. You should still the following message :

   ![image](https://github.com/user-attachments/assets/ebd228ce-2b2f-4840-a786-96629ce11040)
   ![image](https://github.com/user-attachments/assets/f917044f-e9ea-49fd-a5c4-b204d2a94962)

2) Stage the contents of a repository using `git add`
   To add untracked or modified files to the staging area, use `git add`.
   When you add the file, you should see the following message:

   ![image](https://github.com/user-attachments/assets/c5ec49cc-fa7c-4723-8714-695b4417aaa6)

   Now, instead of adding a file, you can also add a directory. You can have multiple files within this directory and to add all files within the directory, simply add the directory to track.

   ![image](https://github.com/user-attachments/assets/eda3a714-f59b-4fd1-a3de-b94bf1d06366)
   ![image](https://github.com/user-attachments/assets/ee71da75-69f1-48c9-a77d-7c3ba31a8a30)
   ![image](https://github.com/user-attachments/assets/1d6c2597-96a4-4fb5-bde9-c5acda6ebd80)
   ![image](https://github.com/user-attachments/assets/f0a43e89-8465-4703-b20d-2994371ce64e)

4) Commit the staged changes using  `git commit`
   Use `git commit -m ` followed by your commit message. If you don't use `-m` flag then a default editor will open to store your commit message.
   `git commit` stores the snapshot of your current project.
   
6) View the commit history using  `git log`
   To see a condensed version use, `git log --oneline`.
   To see only 5 recent commits instead of all, use `git log -5`
   
# Remote Repository:
Generally represented by `origin`
1) Cloning vs Adding a remote repository
   When you don't have a local repository, then you `clone` the remote.
   When you have a local repository, then you `add` the remote.

# General Tips:
1) To add all untracked or modified files, use `git add .`
2) To display information about remote repository, use `git remote --verbose` or `git remote -v`
3) To add a remote repository to an local repository, run the command `git remote add origin <url-of-the-remote-repository>` inside your local repository.
   Here, `origin` will be the alias for the url provided.
4) To push local commits to remote for the first time, use `git push [-u] [<repository(name/alias)/URL>] [<branch>]`.
   `-u` is used to track the branch. You can use `-u` or `--set-upstream`.
   For e.g.: `git push -u origin master`.
   Note: Everything within `[]` is optional. Without it, git will use the defaults which are the previous values used when you first pushed to a remote branch.
6) To push a local repository's branch to a new repository, different from the origin remote repository:
   ```
   git push [--set-upstream] [url to the new repository] [branch-name]
   ```
   
