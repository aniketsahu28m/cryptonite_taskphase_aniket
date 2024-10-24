### Untangling Users

#### Becoming root with `su`
I switched to the root user by running `su` in the terminal and entering the root password `hack-the-planet`. After becoming the root user, I used `cat /flag` to read the contents of the file.

#### Other users with `su`
I switched to the user `zardus` by running `su zardus` and entered the password `dont-hack-me`. Once I became the user `zardus`, I ran `/challenge/run` to execute the command.

#### Using `sudo`
To access the contents of the `flag` file as the root user, I ran `sudo cat /flag` in the terminal.
