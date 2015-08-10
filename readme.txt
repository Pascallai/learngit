Hi github
This is the first file to github.

This is what i want to do with github:
1. Manage axure files;
2. Manage icon designs;

Plans of using github:
1. I will add some icons, try to make some changes and repost to repostory;

Methodes of using github:

Before all:
git config --global user.name "someone"
git config --global user.email "someone@someplace.com"

1. Download github install files;
2. Install it and get git bash running;
3. Use command "mkdir foldername" to creat git repostory;
4. Use command "git init" to initialize the repostory;
5. Drag your files to your repostory, use command "git add" add file to repostory;
6. Use command "git commit -m "xxx"" to apply the action.

this is for now.

See log files:
$ git log
$ git log --pretty=oneline

See all logs:
$ git reflog

Rollback to the a version:
$ git reset --hard HEAD^
$ git reset --hard HEAD~100
$ git reset --hard commit_Id

