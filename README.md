# Git & GitHub Workflow Assignment

A small static website (`index.html`, `about.html`) used to demonstrate a complete Git workflow:
local repository → commits → branching and merging → `.gitignore` → undoing a commit → pushing to GitHub.

## What each commit demonstrates

| Step | Operation | Commit |
|------|-----------|--------|
| 2.1 | Initial state of the project | `ac56d5d` Initial commit: add index.html and about.html |
| 2.2 | Second commit on `main` (index.html modified) | `15f1be5` Update index.html: add navigation bar and topics list |
| 2.3 – 2.5 | Branch `feature` created, checked out, change committed on it | `e433eab` Add workflow steps section to about.html |
| 2.6 – 2.7 | Back on `main`, `feature` merged with `git merge --no-ff` | `19bbac4` Merge branch 'feature' into main |
| 3 | `.gitignore` ignoring `*.log` files and the `temp/` folder | `c0efae8` Add .gitignore to ignore .log files and temp/ folder |
| 4 | Additional commit ... | `c41c0e3` Add draft contact page |
| 4 | ... undone with `git revert` (history is kept) | `09a5e00` Revert "Add draft contact page" |
| 6 | Command documentation | Add git_commands.txt and README.md documenting all Git commands |

```
*   19bbac4 Merge branch 'feature' into main
|\
| * e433eab (feature) Add workflow steps section to about.html
|/
* 15f1be5 Update index.html: add navigation bar and topics list
* ac56d5d Initial commit: add index.html and about.html
```

Branches on GitHub: `main` and `feature`.

Every command used, with a short explanation, is listed in [`git_commands.txt`](git_commands.txt).
