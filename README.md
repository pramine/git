# git CheatSheet
```
Basic Commands
```
]#git add [directory_or_file]  
	Stage all changes in <directory/file> for the next commit.
]#git commit -m <commit_message>
	Commit the staged snapshot, but instead of launching a text editor.
]#git status 
	List which files are staged, unstaged, and untracked.	
]#git log 
	Display the entire commit history using the default format.
]#git log --follow <file>
	Lists version history for a file, including renames.


```
Configure Git
```
]#git config --global user.name "<name>"
	Sets the name you want atached to your commits
]#git config --global user.email "<email address>"
	Sets the email you want atached to your commits.
]#git config --global --edit
	Open the global configuration file in a text editor/in CLI.

```
Create a New Repo
```
]#git init <directory> 
	Create empty Git repo in specified directory. 
	Run with no arguments to initialize the current directory as a git repository.
]#git clone <repo>
	Clone a remote git repo via HTTP or SSH.

```
Git Branches
```
]#git branch
	List all of the branches in your repo.
]#git branch <branch_name>
	To create a new branch with the name <branch_name>.
]#git checkout <branch_name>
	Switch to an existing branch.
]#git checkout -b <branch_name>
	Create and check out a new branch named <branch>
]#git merge <branch_name> 
	Merge <branch_name> into the current branch.
]# git branch -d <branch-name>
	Deletes the specified branch.

```
Synchronize Changes
```
]#git pull <remote> 
	Fetch the specified remote’s copy of current branch and immediatelymerge it into the local copy.
]#git push <remote> <branch>
	Push the branch to <remote>, along with necessary commits and objects. 
	Creates named branch in the remote repo if it doesn’t exist.
```
git diff
```
]#git diff <first-branch>...<second-branch>
	Shows content differences between two branches.
]#git diff HEAD 
	Show difference between working directory and last commit.
]#git diff --cached 
	Show difference between staged changes and last commit
