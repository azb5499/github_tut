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

[W3Schools Github tutorial](https://www.w3schools.com/git/git_remote_getstarted.asp?remote=github)

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
- Github pages
  1. Create a new repo
  2. Save the repo's name with the trailing file extension of `.github.io`
  3. Connect repo to computer the normal way. The whole `git remote add origin LINKTOREPOHERE`
  4. Push changes or files to Github
  5. Confirm files existence
  6. Check the pages settings for the repo and the link to the github page hosting the website should be there.
- Github fork
  1. Select a repo of someone elses you wish to copy or work on yourself or contribute to theirs.
  2. At the top right hand corner you should see an option called `fork`
  3. Select `fork` and this will then be added to your accounts repositories.
  4. You have succesfully created a fork of someone elses repo.
- Cloning a repo

```
Repos can be either be cloned to keep a copy of on your local machine or contribute to someone elses github repo.
```

  1. Navigate to the folder you wish to store this git repo in. Open a git bash window here.
  2. Once a fork has been created of desired repo on github. Select the `Code` button of the original repo that was cloned from and copy the repo URL.
  3. Run the `git clone LINKTOREPOHERE` command which will copy the repo to your local machine.
  4. Test if the file is in the location specified by using dir/ls or by checking file explorer at location.
  5. Verify if all commit history is present by using `git log`.
  6. Run the `git remote -v` command to check all remotes.
  7. Configure the current remote from `origin` (the most likely name since origin is the name of a repo you own on github and since this was copied from someone elses repo that they owned and doesnt belong to us, by convention we have to rename this remote to `upstream`)
     1. Run `git remote rename origin upstream`. Origin can be replaced with whatever they named their repo but most likely it will be named origin.
     2. check the name by running `git remote -v`.
  8. Fetch the URL of the fork on your GitHub account.
     1. Navigate to your account and the fork you created.
     2. Select the code button and copy the repo URL.
     3. Run `git remote add origin LINKGOESHERE`.
     4. Run `git remote -v` to check if process was successful.

- Github pull requests
  1. Commit changes made to the local repo.
  2. Push the changes made to the remote repo, our own fork.
  3. Create a pull request from the forked repo to the original repo.
  4. Add custom notes to explain what the pull request is about.
  5. Submit pull request.
  6. Members who have access to original repo can view the pull request, approve, comment and merge.
- .gitignore
  1. navigate to project route folder.
  2. run the `touch .gitignore` command.
  3. Open the `.gitignore` file and enter the names of the files that you want git to not track.
  4. For file types you can type `*.FILEEXTENSION`. e.g. `*.png`. This will ignore all png files.
  5. for folders you can type `FOLDERNAME/`. e.g. `images/` this will ignore everything in the images folder.
