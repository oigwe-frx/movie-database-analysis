# GitHub Rules of Engagement

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


## **Adding Changes:**

1. Open your terminal or command prompt.
2. Navigate to the local directory of your Git repository, where you have made changes.

3. Use the `git status` command to see the changes you've made. This will show you a list of modified, untracked, and staged files.

4. To stage the changes you want to commit, use the `git add` command followed by the filenames or directories:

   ```
   git add <file1> <file2> ...
   ```

   Alternatively, you can use `git add .` to stage all changes in the current directory.

**Committing Changes:**

5. Once you've staged your changes, commit them with a descriptive commit message:

   ```
   git commit -m "Your commit message here"
   ```

   Replace `"Your commit message here"` with a meaningful message that describes the purpose of your commit.

**Pushing the Branch:**

6. After committing your changes locally, you can push your branch to the remote GitHub repository. Use the following command:

   ```
   git push origin <branch_name>
   ```

   Replace `<branch_name>` with the name of the branch you want to push. If you've created a new branch, this will typically be the same name as the branch you created earlier.

7. Git will prompt you for your GitHub credentials if you haven't already authenticated.

8. Once the push is complete, your changes will be pushed to the remote branch on GitHub.

Your changes are now updated in the remote branch on GitHub. Keep in mind that other collaborators can also see and work with these changes if they have access to the same repository and branch.

## **Opening a PR:**
Opening a Pull Request (PR) in a Git repository, particularly on platforms like GitHub, is a common way to propose changes to a codebase. Here are the rules and best practices for opening a PR:

1. Push Your Branch:

Push your branch with the changes to your forked repository on GitHub using the git push command.

2. Create the Pull Request:

Visit the original repository on GitHub and click on the "New Pull Request" button.
Select the base branch (usually the main or development branch) and the branch with your changes as the compare branch.
Provide a clear and descriptive title and description for your PR. Explain what the changes do and why they are necessary.

3. Review and Collaboration:

Collaborate with other contributors, if applicable. Respond to feedback and make necessary changes to your code.
Ensure that your code passes any required tests or code reviews.

4. Keep Your PR Updated:
- If the base branch changes while your PR is open, update your PR branch and resolve any conflicts if necessary.

5. Be Patient and Responsive:
- Be patient while waiting for reviewers to provide feedback. Respond promptly to comments and maintain good communication with the reviewers.

6. PR Approval and Merge:
- Once your PR has received approval from maintainers or reviewers, it can be merged into the main or development branch. In some projects, maintainers will handle the merging process.

Following these rules and best practices will help ensure a smooth and effective contribution process when opening a Pull Request in a Git repository.

## **Branch naming:**
Branch naming conventions are essential for maintaining a well-organized and easily understandable codebase in a collaborative environment. Here are some best practices for branch naming:

1. Use Descriptive Names:

Branch names should be descriptive of the changes or the feature you are working on. A clear and concise branch name makes it easier for others to understand its purpose.

2. Start with a Prefix:

It's a good practice to start your branch names with a prefix to indicate the type of branch. Common prefixes include:
feature/: For new feature development.
bugfix/: For fixing bugs.

3. Use Dashes or Underscores:

Use dashes (-) or underscores (_) to separate words in branch names. For example, feature/user-authentication or bugfix/fix-css-bug. Avoid using spaces or special characters.

4. Lowercase Letters:

Keep branch names in lowercase for consistency and to avoid potential issues on case-sensitive file systems.

5. Keep it Short and Meaningful:

Branch names should be short but convey their purpose clearly. Avoid excessively long branch names that may be difficult to read and manage.

6. Avoid Special Characters:

Avoid using special characters like ~, ^, *, or ? in branch names, as they can cause issues with some Git tools and systems.
Use Consistent Terminology:

Establish consistent terminology across your team or project to standardize branch naming conventions. This makes it easier for everyone to understand and follow.


Examples of well-named branches following these practices:

feature/context-paragraph
bugfix/fix-namingerror-section-3

By following these best practices, you can create branch names that are both informative and consistent, making it easier to collaborate and manage your Git repository effectively.


## **PRs:**

1. Use Descriptive Titles:

Provide a clear and descriptive title for your PR. It should summarize the purpose of the changes you've made. A well-crafted title makes it easier for reviewers to understand what the PR is about.
Provide Detailed Descriptions:

In the PR description, explain the problem you are solving, why it's necessary, and how you've addressed it. Include any relevant context or links to issues, tasks, or documentation. The more information you provide, the easier it is for reviewers to evaluate your changes.

2. Keep PRs Focused:

Each PR should address a single, well-defined issue or feature. Avoid combining unrelated changes in a single PR, as it can make reviews more complex and increase the likelihood of merge conflicts.
Keep Code Changes Concise:

Focus on the changes required to address the issue or implement the feature. Avoid including unrelated code modifications in the same PR.

3.Follow Coding Standards and Style Guidelines:

Ensure that your code adheres to the project's coding standards, formatting guidelines, and style conventions. Consistency is crucial for maintainability.

4.Test Your Changes:

Before creating a PR, thoroughly test your changes to ensure they work as expected. Include automated tests, if applicable, and provide instructions for manual testing if necessary.
Check for Merge Conflicts:

Before creating a PR, pull the latest changes from the target branch (usually the main or development branch) and resolve any merge conflicts locally to avoid complicating the review process.

5. Request Reviews:

Assign reviewers who are knowledgeable about the codebase and the changes you've made. Multiple sets of eyes help identify issues and improve the quality of the code.

6. Respond to Feedback Promptly:

Be responsive to feedback from reviewers. Address comments, questions, and concerns in a timely manner. Engage in constructive discussions to reach a consensus.
Ensure CI/CD Pipelines Pass:

Make sure that your changes pass any automated Continuous Integration (CI) or Continuous Deployment (CD) pipelines and tests defined for the project.
Avoid Force Pushing to the Branch:

Once your PR is open, avoid force pushing (overwriting) changes to the same branch. This can disrupt the review process and cause confusion.

7. Use Labels and Milestones (if applicable):

Some platforms, like GitHub, allow you to use labels and milestones to categorize and track PRs. Use these tools to provide additional context and organization.
Keep PRs Updated:

If there are changes requested by reviewers or if the base branch has been updated, ensure your PR remains up-to-date by rebasing or merging the latest changes.
