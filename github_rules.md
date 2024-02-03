# Github

## **Cloning a GitHub Repository:**

1. Open your terminal or command prompt.
2. Navigate to the directory where you want to clone the repository. You can use the `cd` command to change directories.
3. Use the following command to clone the repository:

   ```
   git clone <repository_url>
   ```

   Replace `<repository_url>` with the URL of the GitHub repository you want to clone. You can find this URL on the GitHub repository's main page.

4. Git will download the repository to your local machine, creating a new directory with the repository's name.

## **Creating a New Branch:**

1. After cloning the repository, navigate to the cloned repository's directory using the `cd` command:

   ```
   cd <repository_name>
   ```

   Replace `<repository_name>` with the actual name of the cloned repository.

2. To create a new branch, use the following Git command, replacing `<branch_name>` with the desired name for your branch:

   ```
   git branch <branch_name>
   ```

   For example:

   ```
   git branch feature/my-new-feature
   ```

3. To switch to the newly created branch, use the following command:

   ```
   git checkout <branch_name>
   ```

   For example:

   ```
   git checkout feature/my-new-feature
   ```

   This command will switch your working directory to the newly created branch, allowing you to make changes specific to that branch.

4. You can now start making changes to the code within your new branch. Once you're ready, commit your changes using `git commit` and push them to the remote repository using `git push`. Your new branch will be created on GitHub when you push the changes.

