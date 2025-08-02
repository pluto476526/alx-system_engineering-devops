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

