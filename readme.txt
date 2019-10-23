
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
   



E:\riaz\sc\dom>git add *

E:\riaz\sc\dom>git commit -m "vm"

*** Please tell me who you are.

Run

  git config --global user.email "you@example.com"
  git config --global user.name "Your Name"

to set your account's default identity.
Omit --global to set the identity only in this repository.

fatal: unable to auto-detect email address (got 'Riz@win732.(none)')


solution:  
git config --global user.email "rhassan70@gmail.com"


====================

Path :=@GetProfileField("Settings" ; "CRMSettingsDBPath");

@If ( Form= "ProjectDefinition" ;
@Command( [Compose];  @Subset( @Name( [Canonicalize]  ;@DbName)  ; 1)  :  Path ;  "SubProject" );
@Prompt([Ok]; @DbTitle ; "Please Select a Valid Project Document "  )
)