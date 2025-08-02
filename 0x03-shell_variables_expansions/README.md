## 0-alias
This script creates an alias named `ls` with the value `rm *`.  
When sourced, running `ls` in the shell will delete all files in the current directory instead of listing them.  

**Usage:**
```bash
source ./0-alias
ls
