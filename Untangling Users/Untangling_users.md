### Untangling Users

#### Becoming root with su
I executed `su` in the terminal to switch to the root user and was prompted to enter the root password.  
After entering the root password "hack-the-planet," I successfully became the root user.  
I then ran `cat /flag` to read the contents of the file.

#### Other users with su
I used `su zardus` in the terminal to switch to the user zardus and was prompted to enter the password.  
After entering "dont-hack-me," I became the user zardus.  
I executed `/challenge/run` to run the command.

#### Cracking passwords
I ran `john /challenge/shadow-leak` to crack the password hashes found in the file `shadow-leak`.  
I obtained the cracked password "aardvark" for the user zardus.  
I then switched to the user zardus again using `su zardus` and entered the password "aardvark."  
After becoming the user zardus, I ran `/challenge/run`.

#### Using sudo
I executed `sudo cat /flag` in the terminal to read the contents of the file flag as the root user.
