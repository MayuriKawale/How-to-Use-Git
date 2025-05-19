This repository is made for people who are getting started to use Git

# Creating a Local Repository:
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

## General Tips:
1) To push a local repository's branch to a new repository, different from the origin remote repository:
   ```
   git push --set-upstream [url to the new repository] [branch-name]
   ```
