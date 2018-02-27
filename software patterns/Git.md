### System Modules

Divide a system into modules, each of which is responsible fro a particular functionality.
* Working directory // one current version of your project
* Staging area // a file table containing what(files or path associated with files) will go into your next commit
* Local repo // store the metadata about the database & objects about your project
     
## System Patterns
Kinds of workflows among modules classify as patterns.
    
Normal commit
1. add/modify files in the working directory
2. stage them to the staging area
3. commit them to the local repo

Remove the files 
from the staging area 

    git rm files|path to files
    
from the working area

    git rm --cached files|path to files
    
Unstage the staged files

    git reset HEAD files|path to files

Revert the last version of the project
     
    git checkout -- files|path to filse     
     
    
    