## Status Commands - These are always safe to execute and don't change the repo.
* git  status                       :  Print the status of the current repo
* git  log                          :  Print a list of the most recent commits
* git  diff                         :  Show all differences between unstaged changes 
                                 :  and the last commit.
* git  remote -v                    :  Show all remotes with name and url.

 ## Repo Commands - These modify the state of the repo in some way but do not modify files
* git  init                         :  Initialize a new repo in the current folder
* git  add MYFILE                   :  Add a file with changes to the staging area to be committed.
* git  add -A                       :  Add all added, removed, or changed files to the staging area.
* git  reset MYFILE                 :  Unstage a file (does not modify the file)
* git  commit -m "Added x,y,z"      :  Commit the staged files to the version history.
* git  remote add name MYURL        :  Add a remote with the given name

 ## Modification Commands - These modify local files.
* git  checkout .                   :  Delete all local changes and restore the last commit.
* git  clone MYURL                  :  Download a remote repo into a folder of the same
                                 :  name. Automatically creates a remote called origin.
* git  clone MYURL foldername       :  Same as above but give the folder a custom name.

 ## Sync Commands - These may modify local and remote files.
* git  push origin master           :  Push all changes to the local 'master' branch
                                 :  to the remote named 'origin'
* git  pull origin master           :  Pull all changes from the remote 'origin' branch
                                 :  to the local branch 'master'.
* git  push -u origin master        :  Same as above but sets 'upstream tracking' to the
                                 :  given branch and remote to enable simple 'git  push'
* git  push                         :  Push to the tracked branch after the push -u command.
* git  pull    :  Pull from the tracked branch after the push -u command.