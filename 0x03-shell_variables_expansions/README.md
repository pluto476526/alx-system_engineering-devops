# 0-alias
This script creates an alias named `ls` with the value `rm *`.  
When sourced, running `ls` in the shell will delete all files in the current directory instead of listing them.  

**Usage:**
```bash
source ./0-alias
ls
```



# 1-hello_you

This script prints `hello user`, where `user` is the current Linux username.
It uses the `$USER` environment variable to dynamically insert the logged-in username.

**Example:**
```bash
$ ./1-hello_you
hello pluto
```



# 2-path

This script appends `/action` to the end of the system `PATH` environment variable.
By doing this, `/action` becomes the last directory the shell searches when looking for executables.



# 3-paths

This script counts the number of directories listed in the `PATH` environment variable.
It takes the value of `$PATH`, replaces `:` with newlines to separate directories, and counts the lines with `wc -l`.



# 4-global_variables

This script lists all the environment variables available in the current shell session.
It uses the `printenv` command and displays the variables in `NAME=VALUE` format.



# 5-local_variables

This script lists:
- All **local variables**
- All **environment variables**
- All **shell functions**
It uses the `set` command to display all variables and functions defined in the current shell session.



# 6-create_local_variable

This script creates a new **local variable** named `BEST` with the value `School`.
The variable is only available in the current shell session and its child processes when sourced.

**Example:**
```bash
$ source ./6-create_local_variable
$ echo $BEST
School
```



# 7-create_global_variable

This script creates a new **global (environment) variable** named `BEST` with the value `School`.
Because it is exported, the variable is available to the current shell session and all child processes.

**Example:**
```bash
$ source ./7-create_global_variable
$ echo $BEST
School
$ bash
$ echo $BEST
School
```



# 8-true_knowledge

This script prints the sum of:
- The number `128`
- The value stored in the environment variable `TRUEKNOWLEDGE`
It uses Bash arithmetic expansion `$(( ... ))` to perform the addition.



# 9-divide_and_rule

This script prints the result of dividing the value of the environment variable `POWER` by the value of the environment variable `DIVIDE`.
It uses Bash arithmetic expansion `$(( ... ))` to perform the division.




# 10-love_exponent_breath

This script calculates `BREATH` raised to the power of `LOVE`, where both are environment variables.
It uses Bash arithmetic expansion `$(( ... ))` with the exponentiation operator `**`.




# 11-binary_to_decimal

This script converts a binary number (base 2) stored in the environment variable `BINARY` to its decimal (base 10) equivalent.
It uses Bash arithmetic expansion with the syntax `base#number`.

