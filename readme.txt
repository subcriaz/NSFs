
<Empty Foldrer are not push to github >


Add new repo NSFs on github

F:\GitHub\NSfs>git init
Initialized empty Git repository in F:/GitHub/NSfs/.git/

git remote add origin https://github.com/subcriaz/NSFs (one time command required )

F:\

>git add *

F:\GitHub\NSfs>git commit -m "sacdsad"
[master (root-commit) 2b9ee7c] sacdsad
 1 file changed, 1 insertion(+)
 create mode 100644 readme.txt

git push origin master

------------------

Now create 2 folders db1 , db2 under NSFs folder 

create 2 nsf files (db1.nsf and db2.nsf )  in desgner and set source control pointing to these folders respectively

right Click 0n db, Team Development - Setup Source Control for this application

add few forms and views in both dbs.


from prject navigator - you will see ... 
right click db, Team development - Synch with NSf , and then Synch with on Disk Project 


Now apply git command to upload on github website  


--------
   
