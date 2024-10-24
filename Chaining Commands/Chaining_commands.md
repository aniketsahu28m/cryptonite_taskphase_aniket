### Chaining Commands

#### Chaining with Semicolons
I ran `/challenge/pwn; /challenge/college` in the terminal to execute both commands sequentially.

### Your First Shell Script

#### Creating a Shell Script
I created a new file `x.sh`. The file contained the following commands:

`/challenge/pwn
/challenge/college`

After saving the file, I ran `bash x.sh` in the terminal to execute the script.

#### Redirecting Script Output
I ran `bash x.sh | /challenge/solve` to pipe the output of the script to the `solve` command.

#### Making Shell Script Executable
Modified `x.sh` to have the following content:
`/challenge/solve`

After running `chmod a+x x.sh` to make it executable, I ran `./x.sh` to execute the script.




