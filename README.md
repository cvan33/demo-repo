# demo

some descriptions!

## Subheader

Know how to commit on git 
cammand:git status
will show all updated, deleted and created files

cmd:git add .
for tack all the file

cmd:git commmit -m
for uploding changes, (-m) for giving message, what & why behind the commiting
if want then give description behind the commit and cmd:git commit -m "Added index.html" -m "some description"

After all this commit happen localy, not live on git

To make it live
cmd:git push
push live on remote repository where project is hosted

SSH keys--

In order to push file under my account then i have to prove to github i'm the owner of the account.
so that have to connect local machine to github account by SSH key.

firt have to generate localy using cmd:SSH-keygen  they specifiy type of encryption, strength of enription and git email address
cmd:ssh-keygen -t rsa -b 4096 -c "kashishsivanisingh@gmail.com 
or another way to connect is set correct remote
first check remote is set or not
cmd:git remote -v 
if return nothing means remote is not set
to set remote
cmd:git remote add origin https://github.com/username/repo.git
or with ssh
cmd:git remote add origin git@github.com:username/repo.git

Git push:
cmd:git push origin master
origin means location of repository
master means branch where want to push

OR
use this 
cmd:git push -u origin main
the -u flag stands for --set-upstream. 
"When I push the main branch to origin (remote), remember this connection, so in the future I can just run git push or git pull without specifying the remote or branch." 
after running cmd:git push -u origin main  this,  later only  just run 
cmd:git push
cmd:git pull


git init
git add .
git commit -m "first commit"
git remote add origin https://github.com/username/repo.git
git push -u origin main


