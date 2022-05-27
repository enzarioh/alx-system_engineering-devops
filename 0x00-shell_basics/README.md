This project contains the following scripts.

0.Prints the absolute path name of the current working directory.
script : echo "#!/bin/bash\npwd">0-current_working_directory

1.Display the contents list of your current directory
script: echo $'#!/bin/bash\nApplications    Documents   Dropbox Movies Pictures\nDesktop Downloads   Library Music Public'>1-listit.sh

2.Changes the working directory to the user’s home directory.
script : $ echo $'#!/bin/bash\ncd ./home '>2-bring_me_home

3. Display current directory contents in a long format
 
Script :$ echo $'#!/bin/bash\nls -l '>3-listfiles

4. Display current directory contents, including hidden files (starting with .). Use the long format.
script : echo $'#!/bin/bash\nls -al '>4-listmorefiles

5. Display current directory contents.
Long format
with user and group IDs displayed numerically
And hidden files (starting with .)

script :$ echo $'#!/bin/bash\nls -l -gu '>5-listfilesdigitonly

6.creates a directory named my_first_directory in the /tmp/ directory.
script : $ echo $'#!/bin/bash\nmkdir -p /tmp/my_first_directory'>6-firstdirectory

7.Move the file betty from /tmp/ to /tmp/my_first_directory.
script : $ echo $'#!/bin/bash\nmv -f betty /tmp/my_first_directory'>7-movethatfile

8. Delete the file betty
script : $ echo $'#!/bin/bash\nrm ~/tmp/my_first_directory/betty'>8-firstdelete

9.Delete the directory my_first_directory that is in the /tmp directory.
script : $ echo $'#!/bin/bash\nrmdir -v my_first_directory*'>9-firstdirdeletion

10.changes the working directory to the previous one.
script :$ echo $'#!/bin/bash\ncd ..'>10-back

11.Script that lists all files (even ones with names beginning with a period character, which are normally hidden) in the current directory and the parent of the working directory and the /boot directory (in this order), in long format.
Script : $ echo $'#!/bin/bash\nls -la . ..'>11-lists

12.Prints the type of the file named iamafile in the /tmp folder.
Script :$ echo $'#!/bin/bash\nfile -f /tmp/iamafile'>12-file_type

13. Creates a symbolic link to /bin/ls, named __ls__ in a working directory.
script :$ echo $'#!/bin/bash\nIn -s /bin/ls _ls_'>13-symbolic_link
 
14.copies all the HTML files from the current working directory to the parent of the working directory, but only copy files that did not exist in the parent of the working directory or were newer than the versions in the parent of the working directory.
Script : $ echo $'#!/bin/bash\ncp -nu *.html ..'>14-copy_html

15.moves all files beginning with an uppercase letter to the directory /tmp/u.
script : 

16.

17.creates the directories welcome/, welcome/to/ and welcome/to/school in the current directory.
Script : $ echo $'#!/bin/bash\nmkdir -p welcome/to/school'>102-tree


