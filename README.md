Git Workflow: Forking, Adding Contributors, and Creating a Pull Request
1. Forking a Repository
Forking a repository allows you to create your own copy of a project on GitHub. Follow these steps to fork a repository and work on it locally:

Steps:
Go to the repository you want to fork on GitHub.
Click the Fork button in the top-right corner of the repository page.
This will create a copy of the repository under your GitHub account.
Clone Your Fork Locally:
After forking, clone the repository to your local machine:

bash
Copy code
git clone https://github.com/YOUR-USERNAME/REPOSITORY-NAME.git
Replace YOUR-USERNAME with your GitHub username and REPOSITORY-NAME with the name of the repository.

2. Adding Contributors
To add contributors to a repository, follow these steps:

GitHub Interface:
Go to the repository on GitHub.
Click on the Settings tab (you must have owner or admin rights).
In the left sidebar, click on Collaborators and Teams.
Enter the GitHub username or email of the person you want to add as a contributor.
Click Add and they will receive an invitation to contribute.
Via Command Line (for adding remote as upstream):
If you are working on a fork and want to keep up with changes in the original repository, you can add the original repository (referred to as upstream) as a remote:

bash
Copy code
git remote add upstream https://github.com/ORIGINAL-OWNER/REPOSITORY-NAME.git
This helps you fetch changes from the upstream repository:

bash
Copy code
git fetch upstream
git merge upstream/main
3. Creating a Pull Request
Once you've made changes to your forked repository, you can create a pull request (PR) to contribute your changes back to the original repository.

Steps:
Make your changes locally.

Commit the changes:

bash
Copy code
git add .
git commit -m "Describe your changes"
Push your changes to your fork (origin):

bash
Copy code
git push origin YOUR-BRANCH-NAME
Go to the original repository on GitHub (the one you forked from).

Click on the Pull Requests tab, then click on New pull request.

Select the base repository and branch (usually main) that you want to merge your changes into.

Select the head repository (your fork) and the branch you pushed your changes to.

Add a description to your pull request and click Create pull request.

By following these steps, you can fork a repository, add contributors, and create a pull request to contribute back to the original project.
