## Matching with *
I used the `cd /ch*` command in the terminal to change the directory to `/challenge`.  
Then, I ran the `/challenge/run` command, which successfully provided the flag.

## Matching with ?
I used the `cd /?ha??enge` command in the terminal, replacing `c` and `l` with `?` to navigate to the `/challenge` directory.  
Afterward, I executed `/challenge/run` and successfully retrieved the flag.

## Matching with []
I ran the `cd /challenge/files` command in the terminal to navigate to the `/challenge/files` directory.  
Next, I executed `/challenge/run file_[bash]` and successfully retrieved the flag.

## Matching paths with []
I executed the `/challenge/run /challenge/files/file_[bash]` command in the terminal, which successfully retrieved the flag.

## Mixing globs
I executed the `cd /challenge/files` command in the terminal to change to the `/challenge/files` directory.  
Then, I ran `ls` to list all the files in the directory, which included:  
- amazing  
- challenging  
- educational  
- great  
- incredible  
- kind  
- magical  
- optimistic  
- queenly  
- splendid  
- uplifting  
- wonderful  
- youthful  
- beautiful  
- delightful  
- fantastic  
- happy  
- jovial  
- laughing  
- nice  
- pwning  
- radiant  
- thrilling  
- victorious  
- xenial  
- zesty  

Next, I tried executing `/challenge/run [cep]`, but since the file did not have an extension, I ran `/challenge/run [cep]*` instead, which successfully retrieved the flag.

## Exclusionary globbing
I navigated to the `/challenge/files` directory by running the `cd /challenge/files` command in the terminal.  
Then, I executed `/challenge/run [!pwn]*` in the terminal, which successfully retrieved the flag.





