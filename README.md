# 2020-02-26-git_collaboration
This is the new title

- `clone`: "Downloading" a repository from cloud to our local computer
  - You only need to do this once just like the `init` command
- `branch <name>`: Create a branch called <name>
  - `checkout <name>` or `switch <name>`: To move `HEAD` (i.e. switch) to that branch
  - `push <branch>` `pull <branch>`: Need to be mindful of which branch we need to push/pull
  `checkout -b <name>`: This will create and checkout the branch at the same time

- Pull Request or PR: Also called merge request is the way to merge branches in the Web UI (e.g. GitHub, BitBucket)
  - This is also where you choose which branch you are going to merge into (default is `master`)
  - In here there is a conversation and "files change" tab where you perform code review
  - When you're ready, click the green "merge pull request" button
  - Don't forget to delete your branch afterward

- Update our local PC
  - Make sure you are on the `master` branch
  - Updte your system with `git pull origin master`
  - `git fetch --prune --all`: This will clean up all your references on all your remotes
  - `branch -d <branch_name>`: This will delete a branch

- Merging branches locally
  - `merge <branch>`: Merges the `<branch>` to the current branch

- Title removal in the master branch
- `rebase` and `cherry-pick` are ways to incorporate other commits in current history or to re-write history
