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
    
  



# JAVASCRIPT
- #### What and why is javascript  ([RESOURCE](https://blog.hubspot.com/website/what-is-javascript))

- #### Execution of js –

   - in browser ( open browser and inspect or console) 
   - js can be run outside of browser using nodejs
   - use <script> tag inside any html doc and run that html file

- #### Variables – var, let and const ([RESOURCE](https://www.javatpoint.com/javascript-variable))
  

- #### Data types  - They are primitive (String, Number, Boolean, Undefined, Null) and non-primitive data types (Object, Arrays)  ([RESOURCE](https://www.programiz.com/javascript/data-types))

- #### Template Literals ([RESOURCE](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Template_literals))

- #### Operators ([RESOURCE](https://www.javatpoint.com/javascript-operators))

                     
- #### String and its methods ([RESOURCE](https://www.javatpoint.com/javascript-string))

- #### Conditional Statements – if , else, else-if , nested if-else switch ([RESOURCE](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/conditionals))

- #### Loops – for , while, do-while, for-in and for-each ([RESOURCE](https://www.javatpoint.com/javascript-loop))

- #### Functions – ([RESOURCE](https://www.javatpoint.com/javascript-function))
  
- #### Arrow Functions  ([RESOURCE](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/Arrow_functions))

- #### Objects ([RESOURCE](https://www.javatpoint.com/javascript-objects))

- #### Arrays ([RESOURCE](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array))

- #### Promise - ([RESOURCE](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise))

- #### Then - ([RESOURCE](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise/then))

- #### Catch - ([RESOURCE](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise/catch))

- #### Finally - ([RESOURCE](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise/finally))

- #### All - ([RESOURCE](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise/all))

- #### async/await – ([RESOURCE](https://exploringjs.com/es2016-es2017/ch_async-functions.html)) ([RESOURCE VIDEO](https://youtu.be/bLre6Uf4Op0))

- #### DOM and BOM ([RESOURCE](https://youtu.be/xOCzjgjedRc))

- #### Classes – read all the sub-topics of Classes also ([RESOURCE](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes)) ([RESOURCE VIDEO](https://youtu.be/7RpdfkSyJfU))

- #### Exception handling – try, catch, throw ([RESOURCE](https://www.w3schools.com/js/js_errors.asp)) ([RESOURCE VIDEO](https://youtu.be/WRNBQCl_cPU))

- #### Strict mode – ([RESOURCE](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Strict_mode))

# HTML & CSS
 #### HTML
- #### DOCTYPE ([RESOURCE](https://www.w3schools.com/tags/tag_doctype.asp)) 
    - What is HTML DOCTYPE? ([video](https://youtu.be/m2-WF_Otq6s))
- #### HTML html Tag ([RESOURCE](https://www.w3schools.com/tags/tag_html.asp))
- #### HTML head Tag ([RESOURCE](https://www.w3schools.com/tags/tag_head.asp))
- #### HTML body Tag ([RESOURCE](https://www.w3schools.com/tags/tag_body.asp))
- #### HTML header Tag ([RESOURCE](https://www.w3schools.com/tags/tag_header.asp))
- #### HTML span Tag ([RESOURCE](https://www.w3schools.com/tags/tag_span.asp))
- #### HTML div Tag ([RESOURCE](https://www.w3schools.com/tags/tag_div.asp))
- #### HTML form Tag ([RESOURCE](https://www.w3schools.com/tags/tag_form.asp))
    - How to structure an HTML form? ([RESOURCE](https://developer.mozilla.org/en-US/docs/Learn/Forms/How_to_structure_a_web_form))
    - Form Data Validation ([RESOURCE](https://developer.mozilla.org/en-US/docs/Learn/Forms/Form_validation))
    - input ([RESOURCE](https://www.w3schools.com/tags/tag_input.asp))
    - textarea ([RESOURCE](https://www.w3schools.com/tags/tag_textarea.asp))
    - basic attributes ([RESOURCE](https://www.w3schools.com/html/html_attributes.asp))
    - action ([RESOURCE](https://developer.mozilla.org/en-US/docs/Learn/Forms/Sending_and_retrieving_form_data))
    - method ([RESOURCE](https://www.w3schools.com/tags/att_form_method.asp))

 #### CSS
 - #### CSS Box Model ([RESOURCE](https://www.w3schools.com/css/css_boxmodel.asp))
      - Learn CSS Box Model ([RESOURCE](https://youtu.be/rIO5326FgPE))
 - #### Grid Systems ([RESOURCE](https://www.w3schools.com/css/css_rwd_grid.asp))
      - Responsive CSS Grid ([RESOURCE](https://youtu.be/68O6eOGAGqA))
 - #### Responsiveness ([RESOURCE](https://blog.froont.com/9-basic-principles-of-responsive-web-design/))
      - Responsive Web Design | 10 Basics ([RESOURCE](https://youtu.be/zF6VSky4SIc))
 - #### Flex-box Model ([RESOURCE](https://www.w3schools.com/css/css3_flexbox.asp))
      - CSS Flexbox ([RESOURCE](https://youtube.com/playlist?list=PLC3y8-rFHvwg6rjbiMadCILrjh7QkvzoQ))
      - Interactively learn flexbox ([RESOURCE](http://flexboxfroggy.com/))
 - #### Frameworks ([RESOURCE](http://flexboxfroggy.com/))
      - Top CSS Frameworks ([RESOURCE](https://youtu.be/N6SXu86bJ6I))
 - #### Pre-processors ([RESOURCE](https://developer.mozilla.org/en-US/docs/Glossary/CSS_preprocessor))
      - CSS Preprocessors ([RESOURCE](https://www.cabotsolutions.com/css-preprocessors-powerful-tools-smarter-styling-web-pages-user-interfaces))
 - #### Sass/SCSS ([RESOURCE](https://sass-lang.com/guide))
      - Understanding CSS, SCSS and SASS ([RESOURCE](https://youtu.be/Q0WJd7JNxEs))
 - #### CSS Post-Processors ([RESOURCE](https://www.hongkiat.com/blog/css-post-processors-tips-resources/))
      - Autoprefixer CSS online ([RESOURCE]([https://sass-lang.com/guide](https://autoprefixer.github.io/)))
  
 - #### CSS Basics ([RESOURCE](https://youtube.com/playlist?list=PLqGj3iMvMa4IOmy04kDxh_hqODMqoeeCy))
 - #### CSS Positioning ([RESOURCE](https://youtube.com/playlist?list=PLqGj3iMvMa4L731ispRfGAabXeRpM4RL6))
  
 - #### CSS Full Course ([RESOURCE](https://youtu.be/OXGznpKZ_sA))
  
# JavaScript ES6
  ([RESOURCE](https://youtube.com/playlist?list=PL4cUxeGkcC9gKfw25slm4CUDUcM_sXdml))
- #### Constants
- #### The Let Keyword
- #### Default Parameters
- #### The Spread Operator
- #### Template Strings
- #### Object Literal Enhancements
- #### New String Methods
- #### Arrow Functions
- #### Sets
- #### Generators
  
  
  
# React
  - #### Folder structure  ([RESOURCE](https://youtu.be/XEO3mFvrDx0))
  - #### React Hooks ([RESOURCE](https://youtube.com/playlist?list=PLC3y8-rFHvwisvxhZ135pogtX7_Oe3Q3A))
  - #### Components ([RESOURCE](https://www.javatpoint.com/react-components))
      - React Components ([RESOURCE](https://youtu.be/GhUjuKVZ9y8))
      - Lifecycle of Components ([RESOURCE](https://www.geeksforgeeks.org/reactjs-lifecycle-components/))
      - React Component Lifecycle([RESOURCE](https://youtu.be/m_mtV4YaI8c))
  - React Hooks - ([RESOURCE](https://youtube.com/playlist?list=PLC3y8-rFHvwisvxhZ135pogtX7_Oe3Q3A))
  - #### State([RESOURCE]Conditional Rendering
      - React State ([RESOURCE](https://youtu.be/Vf6G8E-Mp5Y))
  - #### Props([RESOURCE](https://www.javatpoint.com/react-props))
      - React Props ([RESOURCE](https://youtu.be/lf4lTlkP7mM))
  - #### Props Validation([RESOURCE](https://www.javatpoint.com/react-props-validation))
      - React Props Validation ([RESOURCE](https://youtu.be/LcTXWJ3zT2U))
  - #### State Vs. Props ([RESOURCE](https://www.javatpoint.com/react-state-vs-props))
      - React State Vs Props ([RESOURCE](https://youtu.be/IYvD9oBCuJI))
  - #### Conditional Rendering ([RESOURCE](https://www.geeksforgeeks.org/reactjs-conditional-rendering/))
      - Conditional Rendering in React JS ([RESOURCE](https://youtu.be/ZeP3Kw-VsGI))
  - #### Lists ([RESOURCE](https://www.geeksforgeeks.org/reactjs-lists/))
      - List Rendering([RESOURCE](https://youtu.be/5s8Ol9uw-yM))
  - #### Keys ([RESOURCE](https://youtu.be/Jh47pOXwGq0))
      - ReactJS - Keys([RESOURCE](https://youtu.be/re5_SiVQru0))
  - #### Form([RESOURCE](https://www.geeksforgeeks.org/reactjs-forms/))
      - Basics of Form Handling([RESOURCE](https://www.javatpoint.com/reactjs-tutorial))
  - #### Router([RESOURCE](https://www.geeksforgeeks.org/reactjs-forms/))
      - React Router([RESOURCE](https://www.javatpoint.com/react-router))
