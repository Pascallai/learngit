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
--------------------------------
Functions:

Add file to stage:
$ git add filename

Pull stage file to HEAD:
$ git commit -m "xxx"

Delete file:
$ git rm filename

See log files:
$ git log
$ git log --pretty=oneline

See all logs:
$ git reflog

Rollback to the a version:
$ git reset --hard HEAD^
$ git reset --hard HEAD~100
$ git reset --hard commit_Id

How github works:
1. C:\Git\learngit is workplace;
2. When using "git add filename", your file will be in stage pool;
3. When using "git commit -m "xxx"", all added files will be submitted to HEAD.
------------------------------------------------------------------------------------------------
Build a connection to the remote Github. 

1.
Create SSH, which id_rsa is private key filename:
each SSH_key refer to a specific machine, each computer who needs to connect to the server, have to create a SSH_key from its own.
$ ssh-keygen -t rsa -C "someone@someplace.com"

2.
Here is where the computer stock the id_rsa file:
C:\Users\Administrator\.ssh

3.
Open and copy the content of id_rsa.pub.

4.
Add to the remote server:
$ git remote add origin git@server-name:path/repo-name.git

Try the connection:
$ ssh -vT git@github.com

5.
Commit the connection:
$ git push -u origin master(first push)
$ git push origin master

