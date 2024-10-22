### Shell Variables

#### Printing Variables
I executed `echo $FLAG` in the terminal to display the value of the variable FLAG, which worked as intended.

#### Setting Variables
I ran `PWN=COLLEGE` in the terminal to assign the value COLLEGE to the variable PWN, and it was successful.

#### Multi-word Variables
I used `PWN="COLLEGE YEAH"` in the terminal to set the variable PWN to "COLLEGE YEAH," achieving the desired result.

#### Exporting Variables
I executed `export PWN=COLLEGE` to make the variable PWN available to child processes.  
Then, I assigned `COLLEGE=PWN` to set the variable COLLEGE to the value of PWN.  
Finally, I ran `/challenge/run` in the terminal, which completed successfully.

#### Printing Exported Variables
I ran `env` to print the environment variables and looked through the output to find the FLAG variable.

#### Storing Command Output
I used `PWN=$(/challenge/run)` to capture the command's output into the variable PWN.  
When I ran `echo $PWN`, it displayed the stored value.

#### Reading Input
I executed `read PWN` in the terminal to read user input and save it in the variable PWN.  
I entered "COLLEGE" when prompted, which allowed me to proceed.

#### Reading Files
I ran `read PWN < /challenge/read_me` in the terminal to read the content of the `read_me` file and store it in the variable PWN, achieving the expected result.
