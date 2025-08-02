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

