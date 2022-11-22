# Getting Started

> Each section should be completed in order from top to bottom because some of the skills build on each other.
# Learn Git
- ### What Is GitHub?
At a high level, GitHub is a website and cloud-based service that helps developers store and manage their code, as well as track and control changes to their code. To understand exactly what GitHub is, you need to know two connected principles:

-Version control
-Git

- ### Install Git ([LINK](https://git-scm.com/downloads))

- ### Create a Local Git Repository
     To create a Git repository, follow the steps below:

1. Open a Git Bash terminal and move to the directory where you want to keep the project on your local machine. For example:

       cd ~/Desktop
       mkdir myproject
       cd myproject/
 
    In this example, we changed the directory to Desktop and created a subdirectory called myproject
  
2. Create a Git repository in the selected folder by running the git init command. The syntax is:

       git init [repository-name]
    
    <img src="Git/img/git init.png" width="700">
    
    Now you have successfully created a local Git repository.

- ### Create a New Repository on GitHub
    GitHub allows you to keep track of your code when you're working with a team and need to modify the project's code collaboratively.

    Follow these steps to create a new repository on GitHub:

    1. Log in and browse to the GitHub home page.

    2. Find the <strong> New repository </strong> option under the <strong>+</strong> sign next to your profile picture, in the top right corner.
     <br></br>
    <img src="Git/img/create-repository-in-github.png">
    <br></br>
    3. Enter a name for your repository, provide a brief description, and choose a privacy setting.
    <br></br>
    <img src="Git/img/github-repository-personalization.png">
    <br></br>
    4. Click the Create repository button.

     GitHub allows you to add an existing repo you have <strong>created locally.</strong> To push a local repository from your machine to GitHub, use the following syntax:
     
       git remote add origin https://github.com/[your-username]/[repository-name.git]
       git push -u origin master
    
    For example:
    <br></br>
    <img src="Git/img/push-local-repo-to-github.png">
    <br></br>
    
- ### Add a File to the Repository
    Git notices when you add or modify files in the folder containing the Git repository but doesn't track the file unless instructed. Git saves the changes only for the files it tracks, so you need to let Git know you want to track changes for a specific file.
    
    You can check which files Git is tracking by running:
    
      git status
      
    <img src="Git/img/git-status-command.png">
    <br></br>
    Git notifies you if you have any untracked files. If you want Git to start tracking a file, run the following command:
    
      git add [filename]
      
    For example:
    
    <img src="Git/img/add-file-to-repository.png">
    <br></br>
    
    In this example, we instructed Git to start tracking changes for the test.txt file. Rerunning the <strong>git status</strong> command shows that Git is tracking the specified file.
    

- ### Unstage Files on Git
    Working with Git usually involves adding all the files to your index to prepare them for a commit. If you want to remove some files from the index before committing, you have to unstage the files in Git.

One way to unstage files on Git is to run the <strong>git reset</strong> command. The syntax is:

      git reset [commit] -- [file_path]
    
    For example:
    
    <img src="Git/img/unstage-file-in-git.png">
    <br></br>


- ### Create a Commit
     After adding the specified files to the staging environment, instruct Git to package the files into a commit using the git commit command. Git then stores that file version. You can review the stored version at any given time.

The syntax is:

      git commit -m "Notes about the commit"
      
   Add a message at the end of the commit to state whether it's a new feature, a bug fix, or anything else. Commits remain in the repository, and they are rarely deleted, so an explanation of what you changed helps other developers working on the project or help you keep track of all the changes.

For example:

     <img src="Git/img/push-commit-on-git.png">
    <br></br>

- ### Undo Last Commit
     Use the revert and reset commands to undo changes and revert to a previous commit.

To undo a published commit, use the following syntax:

      git revert [hash]
    
A hash is a code that identifies each commit. Obtain a commit hash by running:

      git log
    
For example:

     <img src="Git/img/undo-last-commit-on-git.png">
    <br></br>

In this example, we first ran the <strong>git log</strong> command to obtain the commit hash and then reverted the last commit by running <strong>git revert</strong> with the commit hash we obtained.

- ### Create a New Branch
The first branch in a git repository is called master, and it is the primary branch in a project.

Creating a new Git branch means creating a copy of the project from a specific point in time. Branches in Git allow users to make new features without applying the changes to the main branch while the feature is in development.

The common method for creating a new branch is by running:

      git branch [new_branch_name]

For example:

     <img src="Git/img/create-a-new-branch-in-git.png">
    <br></br>

In this example, we create a new branch named new-feature.


- ### Switch Branches
Having several branches of a Git project provides a test environment for developers to track progress without affecting the production version of an application. Git allows you to switch between branches with the <strong>checkout</strong> command easily. The syntax is:

      git checkout [branch_name]

Replace [branch_name] with the branch name you want to access.

For example:

<img src="Git/img/switch-branch-in-git.png">
<br></br>
    
- ### Rename a Local or Remote Git Branch
In Git, you can rename a local or remote Git branch.

The syntax for changing a local Git branch name is:

      git branch -m new-name

For example:

<img src="Git/img/change-branch-name-in-git.png">

In this example, we changed the local branch name from new-feature to feature-testing.

Since there isn’t a way to directly rename a remote Git branch, you first need to delete the old branch name, then push the new branch name to the remote repository.

- ### Delete a Local or Remote Git Branch
You may decide to delete a Git branch after merging the changes with the master branch or if the branches become corrupted.

You can delete local and remote Git branches.

Deleting a local branch doesn't affect a remote branch. To delete a <strong>local</strong> Git branch, run:

      git branch -d [branch_name]
      
   Use the following syntax to delete a remote Git branch:
   
      git push [remote_project] --delete [branch_name]
      
   In this example, we deleted a local Git branch:
   
   <img src="Git/img/delete-a-branch-in-git.png">

- ### Set Upstream Branch
Sending something upstream in Git means that you are sending it back to the repository owner.

Using the <strong>git set upstream</strong> command, you can choose the flow direction of your current local branch. The command also allows you to change the default remote branch.

   <img src="Git/img/set-upstream-branch-in-git.png">

Our tutorial on What Is Git Upstream and How to Set an Upstream Branch deals with the different methods for setting an upstream branch and gives a detailed explanation on the topic.

