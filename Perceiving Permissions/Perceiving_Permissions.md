## Perceiving Permissions

### Changing File Ownership
Ran `chmod hacker /flag` to change the file's ownership to the user hacker, then attempted to execute `/flag` but encountered a permission denied error. After running `ls -l` to inspect permissions, I saw the file was owned by hacker with only read and write access for the owner. I used `cat /flag` to read the file contents successfully.

### Groups and Files
Executed `chgrp hacker /flag` to update the group ownership to hacker. Used `cat /flag` to read the file's content afterward.

### Fun with Group Names
Checked group information with `id`, found hacker's group as `grp25436`, and used `chgrp grp25436 /flag` to change the group of `flag` accordingly. Verified with `cat /flag`.

### Changing Permissions
Added read permissions for others with `chmod o+r /flag` and accessed the file content again using `cat /flag`.

### Executable Files
Ran `ls -l /challenge/run` to check permissions on `run`, saw that the file lacked execute permissions for the owner. Added execute permissions with `chmod u+x /challenge/run`, then successfully executed `/challenge/run`.

