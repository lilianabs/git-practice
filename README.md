# GitHub Session for Technical Writers

This is a dummy repository to practice making a Pull Request (PR).

The following sections explain the tasks that you need to perform to create a PR:

* Step 1: Create a Local Copy of the Remote Repository
* Step 2: Create a New Branch
* Step 3: Create a Pull Request in the Original GitHub Repository

## Step 1: Create a Local Copy of the Remote Repository

To create a local copy of a remote repository:

1. Go to the GitHub repository.
1. Click the ![fork](images/fork.png) button located on the top right of the GitHub repository.

    You have a copy of the repository on your GitHub account.

1. Go to your copy of the repository in GitHub (forked repository).
1. Click the ![clone](images/clone-or-download.png) button.
1. Click the ![copy-url](images/copy-url.png) button to copy the repository’s URL address.
1. Open your terminal application.
1. Change the current working directory to the location where you want to store the repository’s contents using the change directory (**cd**) command.
1. Enter `git clone`, and then paste the URL you copied in Step 5. 


## Step 2: Create a New Branch
You need to create a new branch to commit the changes you make to your local copy of the GitHub repository. 

To create a new branch and commit changes to it:

1. Open your terminal application.
1. Change the current working directory to the location where you stored the repository’s contents using the change directory (**cd**) command.
1. Create a new branch:
   
   ```
    git checkout -b name-for-your-branch
   ```
   
     A message informing you that git switched to the branch `name-for-you-branch appears`.
   
   > **Suggestion:** Create a meaningful name for your branch so that you can easily remember what you modified or added to the repository.

1. Stage your changes:

   ```
    git add .
   ```

1. Commit your changes:

   ```
    git commit -m "added/modified a file"
   ```
   >**Note:** Replace the text enclosed in `"..."` with some brief explanation of the additions or modifications you performed to the local copy of the repository.


## Step 3: Create a Pull Request in the Original GitHub Repository
Finally, you need to push your changes to the local copy of the repository created in the [previous step](#step-2-create-a-new-branch) and create a PR in the original GitHub repository that you forked.

To create a a Pull Request in the original GitHub repository:

1. Open your terminal application.
1. Change the current working directory to the location where you stored the repository’s contents using the change directory (**cd**) command.
1. Verify that you are inside the branch you created:

   ```
    git status
   ```

   >**Note:** You can the current branch to a different one by running the command `git branch name-for-you-branch`.

1. Push your changes (commited in the branch you created) to the master branch of the original GitHub repository:

   ```
    git push origin name-for-you-branch
   ```

1. Go to your copy of the repository in GitHub (forked repository).
1. Click the ![new-pull-request](images/new-pull-request.png) button.
1. Select the `name-for-your-branch` branch.
1. 