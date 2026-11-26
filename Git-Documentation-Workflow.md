# Documentation Workflow Using Git



## Introduction



Technical writers create and maintain documentation to help users understand products, features, and processes.



Git helps technical writers track document changes, maintain different versions, and collaborate with other contributors.



This guide explains a basic workflow for managing documentation using Git and GitHub.



## Documentation Workflow



### 1. Create or Edit Documentation



Create a new Markdown file or open an existing document. Write clear, accurate, and well-structured content.



### 2. Check Document Changes



Use the following command to check which files have been modified:



`git status`



### 3. Stage Changes



Use `git add` to prepare the modified documentation for a commit:



`git add filename.md`



### 4. Commit Changes



Save the staged changes in the local repository:



`git commit -m "Updated documentation"`



### 5. Push Changes to GitHub



Upload your committed changes to the remote repository:



`git push origin main`

### 6. Create a Documentation Branch

Before making documentation changes, create a separate branch:

`git switch -c documentation-update`

This keeps documentation work separate from the main branch and allows changes to be reviewed before merging.

### 7. Review and Create a Pull Request

After pushing the documentation branch to GitHub, create a Pull Request (PR).

A Pull Request allows other contributors to review documentation changes before merging them into the main branch.

Reviewers can check:

- Content accuracy
- Grammar and spelling
- Clarity and readability
- Markdown formatting
- Completeness of instructions
### 8. Merge the Documentation Changes

After the Pull Request is approved, merge the documentation branch into the main branch.

Once the merge is complete, update your local main branch:

`git switch main`

`git pull origin main`

This ensures your local repository contains the latest documentation changes.

