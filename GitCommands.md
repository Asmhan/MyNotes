## Git
```bash
git config --global user.name "<Your Full Name>"
git config --global user.email "<your-email-address>"
git config --list
git clone <Project-URL> <optinal-new-name>
git status

git log  
git log --oneline  
git log --stat 	#show the how many files were changed and the number of lines that were added/removed  
git log -p || --patch  
git log -p --stat  
git log -p -w 			# ignore white-space  
git log -p fdf5493 		# show log starting from this commit  
git show 				# show last commit, show same info as git log -p  
git show fdf5493  
git show --stat  
git show -w  
git add <file1> <file2> … <fileN>  
git add .  
git rm --cached <file-name>  
git commit  
git commit -m 'commit message'  
git commit (-a -m || -am) 'commit message'  
git diff  git tag (-a || --annotate) <tag>  
git tag -a <tag> <sha>  
git tag (-d || --delete) <tag>  
git tag

git branch  
git branch <new-branch-name>  
git branch <new-branch-name> <sha>  
git branch -d <branch-name>  
git branch -D <branch-name>  
git checkout <banch-name>  
git checkout -b <branch-name> <from>  
git log --oneline --decorate --graph --all  
git merge <name-of-branch-to-merge-in>  
git commit --amend  
git revert <sha>  
git reset (--soft || --hard)<reference-to-commit>  
``` 
## GitHub
```bash
git remote  
git remote -v  
git remote add <remote-name> <remote-address>  
git push -u <remote-name> <local-branch-name>  
git push -f <remote-name> <local-branch-name>	#f: force
git pull <remote-name> <branch-to-pull>  
git fetch <remote-name> <branch-to-pull>  

git shortlog
git shortlog -s -n
git log --autor=<name-part>
git show <sha>
git log --grep=<regex>

git remote rename <old-name> <new-name>
git rebase -i HEAD~3		#i: interactive

```
