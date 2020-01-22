## Useful commands

```
docker-compose pull && docker-compose up -d
docker logs -f gitlab
ssh -p 6022 -T git@gitlab.example.net  <<Test command
git --version
git config --list
git remote -v
git remote rename <old_name> <new_name>
git status
git add <FILE_NAME>
git reset HEAD <FILE_NAME>             << To unstage
git commit -a 
git commit -a -m "Description of the change"
git commit
git log
git log -p
git log --pretty=oneline
```

```
git branch
git branch <branch_name>
git branch -d <branch_name>
git checkout <branch_name>
```
