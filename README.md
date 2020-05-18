# Welcome the Rehabilitation Robatic Lab Github Training!

There are 2 major con

In this section, you will learn how to use **Github flow** to efficently editing the exsiting files on our repo. 

There are 3 ways we can make a contribution to the repo.
On github https://www.youtube.com/watch?v=sz6zfrQpCQg&list=PLg7s6cbtAD147DXcVp899Fk6SegoLY9gL&index=1
with Commendline

<details><summary>Commend line</summary>
  
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
      cd edit_training
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

## Step 7: Respond to a review

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
    <yourname> has fininshed this editing training.
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

## Step 8: Merge your pull request

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


<hr>
</details>



