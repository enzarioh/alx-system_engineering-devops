0x03. Shell, init files, variables and expansions scripts.

0.Creates an alias.
Name: ls
Value: rm *
script: 

1.Prints hello user, where user is the current Linux user.
echo "hello $USER"

2.Add /action to the PATH. /action should be the last directory the shell looks into when looking for a program.
$ echo $'#!/bin/bash\nexport PATH=$PATH:/action'>2-path

3. Counts the number of directories in the PATH.
 echo $'#!/bin/bash\necho $PATH | tr -s ':' '\n' | wc -1'>3-paths

4. 

5.


6

7.Global variable
 $ echo $'#!/bin/bash\nexport BEST="School"'>7-create_global_variable

8.

9.Prints the result of POWER divided by DIVIDE, followed by a new line.
$ echo $'#!/bin/bash\necho $((POWER / DIVIDE))'>9-divide_and_rule


10.Displays the result of BREATH to the power LOVE
$ echo $'#!/bin/bash\necho $((BREATH ** LOVE))'>10-love_exponent_breath   

11.Converts a number from base 2 to base 10.
"$((2#$BINARY))"

12.Prints all possible combinations of two letters, except oo
$ echo $'#!/bin/bash\necho {a..z}{a..z} | tr " " "\n" | egrep -v "oo"'>12-combinations


13.prints a number with two decimal places, followed by a new line.
$ echo $'#!/bin/bash\nprintf '%.2f\n' $NUM'>13-print_float




