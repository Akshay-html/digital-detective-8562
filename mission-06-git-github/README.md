# Mission 06 - Git and GitHub

## 1. Task / objective

AI-assisted draft: practise status, staging, commits, history, branches, and Pull Requests. The `update-about` branch and Pull Request are created; review the learning bullets and rephrase them yourself before submission.

## 2. Work completed

Added a “My Learning” section to the root README on branch `update-about`. A Pull Request from `update-about` into `main` is required; it must not be merged unless the instructor asks.

### Git command glossary

| Operation | Command | Purpose |
|---|---|---|
| Initialise | `git init` | Starts a Git repository in a folder. |
| Check status | `git status` | Shows changed, staged, and untracked files. |
| Stage selected files | `git add README.md` | Selects changes for the next commit. |
| Commit | `git commit -m "message"` | Records staged changes in local history. |
| View history | `git log --oneline` | Shows recent commits in compact form. |
| Create/list branch | `git switch -c update-about` / `git branch` | Creates or lists a separate line of work. |
| Switch branch | `git switch main` | Moves the working copy to another branch. |
| Publish branch/commits | `git push -u origin update-about` | Sends local commits to GitHub. |
| Retrieve remote changes | `git pull` | Fetches and integrates remote changes into the current branch. |

Staging selects which edits will go into the next commit; a commit records the selected edits in local history. A branch lets work develop separately. A Pull Request proposes reviewing and combining one branch into another.

## 3. Commands / tools used

`git status`, `git add`, `git commit`, `git log --oneline`, `git switch -c update-about`, `git push`, and GitHub CLI for the Pull Request.

## 4. My understanding

Reference note: commits are snapshots of staged changes; pushes publish local commits to GitHub. Branches isolate work until a Pull Request is reviewed. Rewrite these points in your own words.

## 5. Difficulties faced

No command failure occurred. The account's personal email was not used; commits use the GitHub no-reply address.

## 6. How I resolved them

Used the repository-specific Git identity `Akshay-html` and its ID-based GitHub no-reply address to avoid exposing an email address.

## 7. Evidence / files

Root `README.md` (“My Learning” section); branch `update-about`; Pull Request link to be recorded after creation.

## 8. Commit details

Commit message: `Add learning summary to root README`.
