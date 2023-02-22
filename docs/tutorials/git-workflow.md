# Follow the Git workflow

Follow these steps to clone a repo, make file changes, and commit them to GitLab.

## Clone the project repo locally

1. Open a Command Prompt and navigate to the directory you want to clone the repo into.

    ```
    cd <DIRECTORY NAME>
    ```

2. In GitLab, navigate to the repo for your project.
3. Click **Clone** and copy the URL.
4. Back in the Command Prompt, enter the following command:

    ```
    git clone <REPO URL>
    ```

The Command Prompt clones the files from the repo into the specified location.

## Create a new branch locally

Create and check out a branch to commit to.

When making changes, *never* commit directly to the `master` branch! Instead, check it out and make changes to them. Then, test and request reviews through a merge request (MR). Once approved, merge them to `develop` and then to `master`.

1. Run the following command to create a new local branch:

    ```
    git checkout -b <NEW BRANCH NAME>
    ```

    The following output should appear in the terminal:

    ```
    Switched to a new branch <NEW BRANCH NAME>
    ```

## Make changes to a project

You're now ready to make changes to the repo files you've cloned:

1. Using Visual Studio Code (VS Code), open the files you need to edit.
2. Once you complete your edits, save your progress.

You can now use the Command Prompt to add these changes to Git.

## Add the project changes to Git

1. Before you add your changes to your project, verify that Git recognizes the changes you made by running the following command to check the status of the files:

    ```
    git status
    ```

    > **NOTE**
    >
    > You may notice that some directories, such as target, aren't added to Git by default. This is due to the presence of a `.gitignore` file, which ignores any files that don't need to be pushed to Git by default.

2. Once verified, you can add them to Git. Run the following commands:

  ```
  git add <NAME OF FILE WITH CHANGES MADE>
  ```

  Alternatively, if there are multiple files that need to be added, you can use `git add .` to add them all at once.

## Commit the file changes to Git

Now that files are added to Git and you checked the status, commit the files.

1. Run the following command:

    ```
    git commit -m '<MESSAGE RELATED TO THE CHANGES>'
    ```

2. Verify the status again to confirm all files are committed:

    ```
    git status
    ```

The terminal should say: `Nothing to commit, working tree clean`. You've just successfully committed to the branch you created. This is all in your *local Git repository*, and needs to be pushed to update GitLab. Remember, the best practice is to commit often. Think of a commit as saving your progress.

## Push the commits

Now that you've made local commits, push them into the repository in GitLab.

1. Run the following command:

    ```
    git push --set-upstream origin <NEW BRANCH NAME>
    ```

Congratulations! You've synced up the GitLab repo with your local Git changes.

## More info

- [Merge request review responsibilities](review-responsibilities.md)
- [Style Guide](../style-guide/best-practices.md)
