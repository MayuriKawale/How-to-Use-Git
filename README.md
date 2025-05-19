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
## General Tips:
1) To push a local repository's branch to a new repository, different from the origin remote repository:
   ```
   git push --set-upstream [url to the new repository] [branch-name]
   ```
