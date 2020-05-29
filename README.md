# Welcome to the Rehabilitation Robotic Lab Github Training!

There are 2 major learning objectives:
1. Contribute to an existing repository on Github
2. Create a brand new repository from scratch
<hr>

## Here are some important links

<details><summary> important links  </summary>

#### Tutorial videos playlist link:
https://www.youtube.com/playlist?list=PL6H7SVJLuTdFzDSSpn5b5fcWc4pGL_6VU


#### Installing git and setting up configurations:
 For Mac: https://www.youtube.com/watch?v=sJ4zr0a4GAs<br/>
 For Windows: https://www.youtube.com/watch?v=eo00v2aw92Y 
 
 

#### Our Github Organization- Rehabilitation Robotics

https://github.com/Rehabilitation-Robotics

 
#### GitHub features - Explore GitHub

https://www.linkedin.com/learning/learning-github/exploring-github

#### Github Flow 

Credit link: https://github.com/SCODEMeetup/scode-repo-template/wiki/GitHub-flow-(branching)

#### [Video]Github Learning Lab: Introduction to GitHub Walkthrough

https://www.youtube.com/watch?v=sz6zfrQpCQg&list=PLg7s6cbtAD147DXcVp899Fk6SegoLY9gL&index=1

#### Github Learning Lab 
https://lab.github.com/<br/>
Introduction to github: https://lab.github.com/githubtraining/introduction-to-github<br/>
Uploading your project to GitHub: https://lab.github.com/githubtraining/uploading-your-project-to-github

#### Github Desktop
https://desktop.github.com/

</details>

## Work Flow
GitHub Flow:
![git-small](https://user-images.githubusercontent.com/6351798/48032310-63842400-e114-11e8-8db0-06dc0504dcb5.png)


## Contribute to an existing repository on Github
  
<details><summary> Command line  </summary>
  
## Step 1: Create a branch

Let’s complete the first step of the GitHub flow: creating a branch <sup>[:book:](https://help.github.com/articles/github-glossary/#branch)</sup>.

<details><summary>Creating a branch</summary>

## Creating a branch

:tv: [Video: Branches](https://www.youtube.com/watch?v=xgQmu81G1yY)

You just learned how to create a branch—the first step in the GitHub flow.

Branches are an important part of the GitHub flow because they allow us to separate our work from the `master` branch. In other words, everyone's work is safe while you contribute.

### Tips for using branches

A single project can have hundreds of branches, each suggesting a new change to the `master` branch.

The best way to keep branches organized with a team is to keep them concise and short-lived. In other words, a single branch should represent a single new feature or bug fix. This reduces confusion among contributors when branches are only active for a few days before they’re merged <sup>[:book:](https://help.github.com/articles/github-glossary/#merge)</sup> into the `master` branch.

<hr>
</details>

### :keyboard: Activity: Your first branch


1. Open your preferred command line interface, which we'll call your shell from now on.
1. Clone this repository:
      ```shell
      git clone https://github.com/Rehabilitation-Robotics/github_edit_training.git
      ```
1. Navigate to the repository in your shell:
      ```shell
      cd github_training
      ```
1. Create a branch, use whatever name you like. Feel free to use the your name (eg. `git branch JasonZ`). 
      ```shell
      git branch <your-branch-name>
      ```
1. Push the branch to GitHub (eg. `git push --set-upstream origin JasonZ`):
      ```
      git push --set-upstream origin <BRANCH-NAME>
      ```


<hr>


## Step 2: Commit a file

:tada: You created a branch!

Creating a branch allows you to make modifications to your project without changing the deployed `master` branch. Now that you have a branch, it’s time to create a file and make your first commit!

<details><summary>Commits 101</summary>

## Commits 101

When you’re finished creating or making changes to a file on GitHub, scroll to the bottom of the page. Then find the "Commit new file" section.

In the first field, type a commit message. The commit message should briefly tell contributors about the changes you are introducing to the file.

### Rules to live by for commit messages:

- Don’t end your commit message with a period.
- Keep your commit messages to 50 characters or less. Add extra detail in the extended description window if necessary. This is located just below the subject line.
- Use active voice. For example, "add" instead of "added" and "merge" instead of "merged".
- Think of your commit as expressing intent to introduce a change.

<hr>
</details>

### :keyboard: Activity: Your first commit

The following steps will guide you through the process of committing a change on GitHub.


1. Check out to your branch:
      ```shell
      git checkout <your-branch-name>
      ```
1. Create a new file named `<yourname>.md`(eg `JasonZhao.md`).
      for Mac 
      ```shell
      touch <yourname>.md 
      ```
      for windows
      ```shell
      copy con <yourname>.md 
      ```
1. Add the following content to your file:
      ```<yourname> did it 
      ```
1. Stage your new file:
      ```shell
      git add <yourname>.md
      ```
      or 
      ```shell
      git add .
      ```
1. After adding the text, commit the change and a commit message, check out the **Commits 101** drop-down, just above these instructions:
      ```shell
      git commit -m "<YOUR-MESSAGE>"
      ```
1. Push your new commit to GitHub:
      ```shell
      git push
      ```


<hr>



## Step 3: Open a pull request

Nice work making that commit :sparkles:

Now that you’ve created a commit, it’s time to share your proposed change through a pull request! Where issues encourage discussion with other contributors and collaborators on a project, pull requests help you share your changes, receive feedback on them, and iterate on them until they’re perfect!

<details><summary>What is a pull request?</summary>

## Pull requests

Let’s think back to the GitHub flow again. You have created a branch, added a file, and committed the file to your branch. Now it’s time to collaborate on your file with other students taking this class. This collaboration happens in a pull request. Check out this video to learn more:

:tv: [Video: Introduction to pull requests](https://youtu.be/kJr-PIfLDl4)
<hr>
</details>

This pull request is going to keep the changes you just made on your branch and propose applying them to the `master` branch.

### :keyboard: Activity: Create a pull request

1. Open a pull request using [this shortcut](https://github.com/jichengnorth/github-slideshow/compare/refs/heads/my-slide?expand=1) or manually as follows:
    - From the "Pull requests" tab, click **New pull request**
    - In the "base:" drop-down menu, make sure the "master" branch is selected
    - In the "compare:" drop-down menu, select "my-slide"
1. When you’ve selected your branch, enter a title for your pull request. For example `Add jichengnorth's file`
1. The next field helps you provide a description of the changes you made. Feel free to add a description of what you’ve accomplished so far. As a reminder, you have: created a branch, created a file and made a commit, and opened a pull request
1. Click **Create pull request**

<hr>

## Step 4: Respond to a review

Your pull request is looking great!

Let’s add some content to your file. Replace line 5 of your file with a quotation or meme and witty caption. Remember: [Markdown](https://guides.github.com/features/mastering-markdown/) is supported.

### :keyboard: Activity: Change your file


1. Check out to your branch:
    ```shell
    git checkout <your-branch-name>
    ```
1. Open the file `training.md`.
1. Add in following message. 
    ```shell
    <yourname> has finished this editing training.
    ```
1. Stage your new changes:
    ```shell
    git add training.md
    ```
   
1. Commit your changes:
    ```shell
    git commit -m "<YOUR-MESSAGE>"
    ```
1. Push your edits to GitHub:
    ```shell
    git push
    ```



**Note** : Can't find the button to edit the file? It may look like a pencil, or it may look like three dots.

## Step 5: Merge your pull request

Nicely done, you! :sparkles:

You successfully created a pull request, and it has passed all of the tests. You can now merge your pull request.

### :keyboard: Activity: Merge the pull request


1. Check out to the `master` branch:
    ```shell
    git checkout master
    ```
2. Merge your branch:
    ```shell
    git merge <your-branch-name>
    ```
3. Push the merged history to GitHub:
    ```shell
    git push
    ```
4. Delete your the branch locally:
    ```shell
    git branch -d <your-branch-name>
    ```

1. Once your branch has been merged, you don't need it anymore. Click **Delete branch**.

<hr>



</details>
<details><summary> Github.com </summary>
 
Please watch video #5: 

</details>

</details>
<details><summary> Github Desktop(GUI) </summary>
 
Please watch video #6: 

</details>

## Create a brand new repository(repo) from scratch

 <details><summary> process flow </summary> 
  
## Step 1: Planning the move

Uploading your project to GitHub gives you the feature-rich tools and collaboration needed to elevate your project to the next level. Not to mention, it's also pretty exciting. If you're doing this for the first time, you have a few options when uploading your project to GitHub. This course will guide you through the necessary steps to upload a local project to be hosted on GitHub.

I know some people like to get straight to the point while others like more information. For those who like more information, be sure to check out the drop-downs like this one :arrow_down:

<details>
  <summary>Why move to GitHub?</summary>
  <hr>

  ### Why move to GitHub?

  You may be wondering what this GitHub thing is all about and why you should use it. If this sounds like you, here are a few reasons to make GitHub your project's new home:

  - **Version control** — Everything on GitHub is stored in [Git](http://git-scm.com), the best version control system around. Version control allows you to experiment and make mistakes in code without messing up your final product.
  - **Keep your code in one place** — Whether you work on multiple computers or just want to get some important projects off your computer, GitHub is the perfect place to store your projects online.
  - **Collaboration** — Once your code is on GitHub, you can invite others to work on your code with you, share it with the world, or send a link to a friend to help you debug a problem.

  <hr>
</details>

### Where is your project?

Most users find it is easiest to upload a project that is already located on their local machine, so **the goal of this first step is to make a local copy of the repository.** First, let's make sure this course is going to give you the right steps:

<details>
  <summary>Is your project on another version control system, such as Mercurial, Subversion, or another Git platform?</summary>
  <hr>

  ### Moving your project from another version control system

  If you are moving your project from another version control system, the steps are a bit different that uploading your project from your local machine. Because of this, we have a dedicated course for migrating your project to GitHub.

  If you are moving your project from Mercurial, Subversion, or another Git platform, join the [Migrating your project to GitHub](https://lab.github.com/courses/migrating-your-repository-to-github) course to migrate your project to GitHub.

  <hr>
</details>

<details>
  <summary>Is your project using version control?</summary>
  <hr>

  ### Is your project using version control

  If you aren't sure whether or not your code is under version control, it probably isn't. However, here are a few tests you can apply to know for certain:

  - Can you view a history of the changes you have made?
  - Can you easily roll back to a previous version of your project?
  - Are you required to provide "messages" or "commits" when you make changes?

  If none of these are true, your project isn't using version control.

  <hr>
</details>

### :keyboard: Activity: Exporting your project

Choose the drop-down below that best fits your current situation or for a printable version of the steps in this course, check out the [Quick Reference Guide](https://lab.github.com/public/uploading-your-project-to-github.pdf).

<details>
  <summary>Your project is already on your local machine</summary>
  <hr>

  ### Your project is already on your local machine

  :sparkles: Terrific! @jichengnorth since you already have the project locally, you are _almost_ ready to move it to GitHub.

  To confirm: You have a project directory on your computer and you want to save it on GitHub.

  - **If this is correct**, close this issue to signal you are finished with this step. I will open a new issue to show you how to optimize your repository for Git operations.  

  - **If this is incorrect**, please use the next drop-down to learn how to export your project to your local machine or join the [Migrating your project to GitHub](https://lab.github.com/courses/migrating-your-repository-to-github) course to migrate your project to GitHub.

  <hr>
</details>

<details>
  <summary>Your project is on a non-version controlled site, such as CodePen or Glitch</summary>
  <hr>

  ### General instructions

  There are many platforms that allow users to create and store projects. We can't cover them all, but we will do our best to cover the more common examples. First, let's cover general instructions:

  - Export your project using the tools available on the current site. This will usually happen via a .zip, or some other compressed format, downloaded directly to your local machine
  - Save the .zip file
  - Extract the .zip file

  Now let's talk about specific platforms:

  #### Exporting from CodePen

  From the main page of your CodePen project:

  1. Click the **Export** button in the bottom right corner
  1. Save the exported .zip file in your local directory
  1. Extract the .zip file

  #### Exporting from Glitch

  From your Glitch project page:

  1. Click the dropdown next to your project name in the top right corner
  1. Select **Advanced Options**
  1. Select **Download Project**
  1. Save the exported file in your local directory
  1. Extract the file
  1. Rename the `app` folder as desired

  <hr>
</details>

## Step 2: Prepare the project

### Working with Binary files

In general, there are two types of files: text files and binary files.

Text files, like most code files, are easily tracked with Git and are very lightweight.

However, binary files like spreadsheets, presentations with slides, and videos don't work well with Git. If your repository already has some of these files, it's best to have a plan in place before you enable Git version control.

You could choose to remove the binary files, or use another tool like [git-lfs](https://git-lfs.github.com/) (Git Large File Storage). We won't get into detail on how to set up git-lfs in this course, but we will talk about `.gitignore` files next, which are key to protecting your code from becoming bloated with binaries.

### Add a `.gitignore`

As we convert your project to a Git repository, it should only include the source code necessary to build or compile your project. In addition to avoiding binaries as we discussed above, you will also want to keep build artifacts out of your version controlled code. 

To do this, you will create a file in your current project named `.gitignore`. Git will use the `.gitignore` to determine which files and directories should not be tracked under version control. The [`.gitignore` file](https://help.github.com/articles/ignoring-files/) is stored in your repository in order to share the ignore rules with any other users that interact with the repository. 

Since the files to be ignored are dependent on the language you are using, the open source community has contributed some great templates for `.gitignore` files in the [`github/gitignore`](https://github.com/github/gitignore) repository.

### :keyboard: Activity: Prepare your repository

1. **Remove any binary files from your repository**.
2. In your local environment, [create a `.gitignore` file](https://help.github.com/articles/ignoring-files/). You can use a [template](https://github.com/github/gitignore) or create your own.  :tada:


## Step 3: Make the move

Having a project already stored locally enables you to move it to GitHub rather quickly. The following activity provides instructions to move your local project to GitHub using various tools. Select the tool you are most comfortable with and get importing :smile:.

### :keyboard: Activity: Moving your local project

1. In the **Code** tab of this repository, copy the URL shown under **Quick Setup**.
1. Follow the instructions below based on what tool you'd like to use locally.

<details>
  <summary>Using the command line</summary>
  <hr>

  ### Using the command line
  1. Go to Github.com. Log in to your account. 
  1. Click the new repository button in the top-right. You’ll have an option there to initialize the repository with a README file, and you can choose to make this repo public or private. Click the “Create repository” button. 
  1. In your command line, navigate to your project directory. Type `git init` to initialize the directory as a Git repository.
  2. Type `git remote add origin https://github.com/Rehabilitation-Robotics/<yourRepo>.git`
  3. Type `git add .`
  4. Type `git commit -m "initializing repository"`
  5. Type `git push -u origin master` to push the files you have locally to the remote on GitHub. (You may be asked to log in.)

  <hr>
</details>

<details>
  <summary>Using GitHub.com</summary>
  <hr>

  ### Using GitHub.com

  1. add a local repository, and then navigating to your local repository.
  1. Go to Github.com, click `Upload Files` drag and drop in the field provided and clicking **Commit to master**
  2. Add the remote by clicking `Repository > Repository Settings...` and pasting the URL from your repository on GitHub into the "Primary remote repository (origin)" field. Click **Save**.
  3. Click **Publish** in the top right corner to push your repository to GitHub.

  <hr>
</details>


<details>
  <summary>Using GitHub Desktop</summary>
  <hr>

  ### Using GitHub Desktop

  **Watch video #6 -- Git tool: Github Desktop** <br>
  <br>
   **A more detailed instrustion**: https://help.github.com/en/desktop/getting-started-with-github-desktop/creating-your-first-repository-using-github-desktop <br>
  <br>
   **If you already have a local git repository**: <br> 
  1. In GitHub Desktop, add a local repository by clicking `File > Add a Local Repository`, and then navigating to your local repository.
  1. Create your first commit by typing a summary commit message in the field provided and clicking **Commit to master**
  2. Add the remote by clicking `Repository > Repository Settings...` and pasting the URL from your repository on GitHub into the "Primary remote repository (origin)" field. Click **Save**.
  3. Click **Publish** in the top right corner to push your repository to GitHub.

  <hr>
</details>

<details>
  <summary>Using Visual Studio Code</summary>
  <hr>

  ### Using Visual Studio Code

  1. In Visual Studio Code, open the folder for your project.
  1. Click the icon on the left for **Source Control**.
  1. On the top of the Source Control panel, click the **Git icon**.
  1. If the files you see match the repository you want to create, click **Initialize Repository**.
  1. Next to the word **CHANGES**, click the symbol of the plus sign to stage all of the changes.
        - This is part of the two stage commit. You can use this staging function to create meaningful commits throughout the development process.
  1. In the box in the Source Control panel, type a commit message. Something like "initial commit - moving project" could work.
  1. Click the checkmark at the top of the Source Control panel.
  1. Open the integrated terminal found under View > Integrated Terminal.
  1. In your command line, type `git remote add origin https://github.com/jichengnorth/github-upload`
  1. In the Source Control Panel, click the expandable three dots that open a menu of options.
  1. When asked if you'd like to publish the branch, click **Okay**.

  <hr>
</details>

<details>
  <summary>Using Atom</summary>
  <hr>

  ### Using Atom

  1. In Atom, open the folder for your project
  1. At the top of your screen, click **Packages**. Select **GitHub**, and then toggle the **Git Tab** from the drop-down menu.
  1. Select **Create Repository** within the Git tab on the right-hand size of your screen.
  1. Select **Init** to accept the default prompt of the pop up window
  1. In the Git tab, you can see that your files are ready for staging. It _should_ be accounted for, but double check to make sure that none of your binaries or files that you listed in the .gitignore are listed in this dialog menu.
          - If they are, double check your .gitignore file to make sure they're included or remove them from your directory.
  1. Select **Stage All**
          - This is part of the two stage commit. You can use this staging function to create meaningful commits throughout the development process.
  1. In the box at the bottom of the Git panel, type a commit message. Something like "initial commit - moving project" could work.
  1. Select **Commit**
  1. Close Atom
  1. In your command line, navigate to your project directory.
  2. Type `git remote add origin https://github.com/jichengnorth/github-upload`
  3. Return to Atom, and select the [Up/Down arrow icon](https://user-images.githubusercontent.com/13326548/36766999-34ff2bb2-1bed-11e8-90c6-3c97d0837244.png) at the bottom of your Git Tab
  4. Click [Push](https://user-images.githubusercontent.com/13326548/36767211-5fd34ce6-1bee-11e8-964a-f49bed227c02.png), above the noted dialog.
  5. Return to your repository, and note a successful push by finding your files on GitHub's code tab.

  <hr>
</details>

<details>
  <summary>Using Eclipse</summary>
  <hr>

  ### Using Eclipse

  1. In Eclipse, from the Eclipse Marketplace, install the [eGit](http://www.eclipse.org/egit/) GitHub plugin.
  2. Open your existing project.
  3. Display the **Git Repositories** window by selecting Window > Show View > Other > Git > Git Repositories.
  3. Click the **Create a Git Repository** button on the Git Repositories pane.
  4. Make changes to your project and create a commit.
  5. Push the master branch.
  5. When asked for a remote, paste the URL you copied earlier.
  6. Click next, and enter the branch name.

  <hr>
</details>

</details>
