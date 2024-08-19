# This is a heading

## Learning goals for today

- Learn the basics of git
- Learn how to use Github
- Learn markdown
- Set up a repo
- Set up vscode for collaborators
- Develop a simple project

---

## Git

- Init
- `--version`
- status
  - `--short`
- log
- add
  - `add .`
  - `add -A`
- commit -m
  - `commit -a -m`
- branch
  - branch `name`
- checkout
  - checkout `-b name`
- merge
  - git merge `name`
  - conflicts
- reset
  - `git reset`. Unstages changes

## Github

- Creating account
- Adding a remote repo
  - git remote add `origin` , `link to repo`
- pushing to a repo
  - git push --set-upstream `origin master`
- Editing directly on github
  - clicking on a file and editing it however then commiting the changes.
- fetch
  - a command that fetches a change from a remote repo but does not merge with the local repo
- merge
  - you know what merge does
- pull
  - git pull `origin`
  - this fetches and merges the latest version of the project from github.
- Creating branches on Github
  1. Go on Github
  2. Click on the master branch
  3. Create the new branch
  4. Pull to local
- Creating branches on local and pushing to git
  1. Create your local branch
  2. Do whatever
  3. Save changes and commit
  4. git push `origin branchNameToCommit`
- Branch
  - `git branch -a`. Shows all branches, local and remote
- Deleting a branch locally then reflecting those changes on github
  - `git push origin --delete branchName`
- Merging pull requests directly on github
  1. Click compare and pull requests
  2. Create pull request
  3. Add additional info and follow steps.
- The GitHub flow
  1. Create a branch for a feature
  2. Make File changes and add commits
  3. Push changes to remote repo
  4. Create a pull request
  5. Review the changes
  6. Deploy branch to check for errors before merging with master
  7. Merge if successful
