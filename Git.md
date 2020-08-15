# Git

## What is Git?

Git is a version control system. It is a protocol. A protocol means that it interoperates with other things that use the protocol. Git is used to maintain file history.

## What is GitHub?

Website used for hosting git projects. it is a place where projects live. Without it you wouldn't have your projects.

## What are Git Hosting Site Examples?

* GitHub
* GitLab
* BitBucket 

## Git Commands

### Status

Shows you the current status of the project. It shows modified tracked and untracked files. Tracked meaning commited files and untracked meaning non-commited files or git doesn't know about.

```bash
% git status
```

### Add

Adds a modified file to a commit.

```bash
% git add Git.md
```

### Commit

Dedicate to a logical unit of work. In other words, when you have completed writing the code for one step of what you're doing, commit to save your progress for later use.

```bash
% git commit -m "Message"
```

### Push

Takes changes from local computer and moves them to remote computer (GitHub).

```bash
% git push
```

### Diff

Shows changes in modified files.

```bash
% git diff Git.md
```

### Pull

Grabs commits from remote (GitHub) 

```bash
% git pull
```

### Branch

Create a new area for work to be committed.

#### To create a branch:

```bash
% git checkout -b my-branch-name # create branch on local
% git push -u # push branch to remote
```
#### To see all branches:

```bash
% git branch -a
```

#### To remove a branch after merging:

```bash
% git checkout master # leave the branch and go back to master
% git fetch -p # tells git what changed on the remote, deletes remote branches that don't exist anymore
% git pull # pull in the merged changes from the branch
% git branch -d my-merged-branch # deletes the merged branch if OK, -D to delete regardless if safe
```