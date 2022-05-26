The below information contains the decription of the scripts

0. My name is Betty: Switches the current user to the user betty 
   Script : echo $'#!/bin/bash\nsu betty'>0-iam_betty.sh
 
1. Who am I : Prints the effective username of the current user.
   script   : echo ' echo $'#!/bin/bash\nwhoami '>1-who_am_i.sh

2. Groups : Prints all the groups the current user is part of.
   script :echo $'#!/bin/bash\nid -Gn '>2-groups.sh

3. New owner :Changes the owner of the file
  script : $ echo $'#!/bin/bash\nchown Administrator hello'>3-new_owner.sh


4. Empty! : Creates an empty file called hello.
  script :$ echo $'#!/bin/bash\ntouch hello'>4-empty.sh


5. Execute : Adds execute permission to the owner of the file hello
script  : $ echo $'#!/bin/bash\nchomd +x hello'>5-execute.sh

6. Multiple permissions : Adds execute permission to the owner and the group owner, and read permission to other users, to the file hello.
Script : $ echo $'#!/bin/bash\nchomd u:g +x hello'>6-multiple_permissions.sh

7. Everybody! : Adds execution permission to the owner, the group owner and the other users, to the file hello
$ echo $'#!/bin/bash\nchomd a +x hello'>7-everybody.sh

8. James Bond : Write a script that sets the permission to the file hello as follows:
Owner: no permission at all
Group: no permission at all
Other users: all the permissions

Script :$ echo $'#!/bin/bash\nchomd o +x hello'>8-James_Bond.sh

9. John Doe : sets the mode of the file hello to this: -rwxr-x-wx 1 julien julien 23 Sep 20 14:25 hello
Script : echo $'#!/bin/bash\nchomd 750 hello'>9-John_Doe.sh

10 . Look in the mirrow :sets the mode of the file hello the same as olleh’s mode.
The file hello will be in the working directory
The file olleh will be in the working directory
Script :$ echo $'#!/bin/bash\nchomd 644 hello'>10-mirror_permissions.sh

11. Directories : adds execute permission to all subdirectories of the current directory for the owner, the group owner and all other users. 
Script : echo $'#!/bin/bash\nchomd ugo +x 0x01-shell_permissions'>11-directories_permissions.sh

12.More Directories : creates a directory called my_dir with permissions 751 in the working directory.
Script :$ echo $'#!/bin/bash\nmkdir my_dir chmod 751 0x01-shell_permissions'>12-directory_permissions.sh

13. Change Group : Changes the group owner to school for the file hello
Script : $ echo $'#!/bin/bash\nchgrp school hello'>13-change_group.sh


