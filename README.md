# Git Workshop

## What exactly is GitHub?

GitHub is a Git repository hosting service, but it adds many of its own features. While Git is a command line tool, GitHub provides a Web-based graphical interface. It also provides access control and several collaboration features, such as a wikis and basic task management tools for every project.

## Git vs. Github

Git is a revision control system, a tool to manage your source code history. GitHub is a hosting service for Git repositories. So they are not the same thing: Git is the tool, GitHub is the service for projects that use Git.

## Cloning a repository:
```
git clone <URL>
```

## List all remotes
```
git remote -v
```

## Adding Remote Repositories
```
git remote add <remote name> <url>
```

## Pushing to Your Remotes
```
git push <remote name> <branch name>
eg: git push origin master
```

## Renaming and Removing Remotes
```
git remote rename <old name> <new name>
```

## Removing a remote
```
git remote remove <remote name>
```

## Rebasing to latest changes
```
git pull --rebase <remote name> <branch name>
```

The git pull command is actually a combination of two other commands, git fetch followed by git merge. In the first stage of operation git pull will execute a git fetch scoped to the local branch that HEAD is pointed at. Once the content is downloaded, git pull will enter a merge workflow. A new merge commit will be-created and HEAD updated to point at the new commit.

The --rebase option can be used to ensure a linear history by preventing unnecessary merge commits. it’s like saying, "I want to put my changes on top of what everybody else has done." 



