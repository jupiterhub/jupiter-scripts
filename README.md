## Installation

Run `cat gitconfig_aliases >> .gitconfig`

## Cheat sheet

The following is a complete list of all aliases included in this configuration.

### Staging & Committing Files

| Alias | Command | Description |
| :--- | :--- | :--- |
| `a` | `add` | Stage a file. |
| `aa` | `add --all` | Stage all changes in the repository. |
| `ap` | `add --patch` | Interactively stage parts of files. |
| `c` | `commit -v` | Commit with a verbose diff shown. |
| `cm` | `commit -m` | Commit with an inline message. |
| `ca` | `commit -v -a` | Commit all tracked files (add + commit). |
| `cam` | `commit -am` | Commit all tracked files with an inline message. |
| `amend` | `commit --amend --no-edit` | Add to the last commit without changing the message. |
| `amendm`| `commit --amend` | Add to the last commit and edit the message. |
| `uns` | `restore --staged` | Unstage a file (the modern way). |

### Branching & Merging

| Alias | Command | Description |
| :--- | :--- | :--- |
| `b` | `branch` | List all local branches. |
| `br` | `branch -r` | List all remote-tracking branches. |
| `bmerged`| `branch --merged` | List branches that have been merged into the current branch. |
|`bnotmerged`| `branch --no-merged` | List branches that have not been merged. |
| `co` | `checkout` | Switch to another branch. |
| `cb` | `checkout -b` | Create and switch to a new branch. |
| `bd` | `branch -d` | Delete a merged local branch. |
| `bD` | `branch -D` | Force delete a local branch. |
| `rebase`| `rebase` | Re-apply commits on top of another base tip. |
| `ri` | `rebase -i` | Begin an interactive rebase. |
| `rc` | `rebase --continue` | Continue a rebase that was paused for conflicts. |
| `ra` | `rebase --abort` | Abort and clean up after a failed rebase. |

### Remote & Network Ops

| Alias | Command | Description |
| :--- | :--- | :--- |
| `f` | `fetch` | Fetch changes from a remote. |
| `l` | `pull` | Fetch and integrate with another repository. |
| `p` | `push` | Push committed changes to a remote. |
| `pf` | `push --force-with-lease` | Force push safely, ensuring no one else has pushed.
