### Pondering PATH

#### The PATH Variable
I cleared the `PATH` variable by running `PATH=""` in the terminal.  
Then, I executed `/challenge/run` to try running the command with the empty `PATH`.

#### Setting PATH
I updated the `PATH` by setting it to `/challenge/more_commands` with the command `PATH=/challenge/more_commands`.  
After that, I ran `/challenge/run` again to execute the command.

### Adding Commands

#### Creating and Adding Custom Commands
I created a file named `win` with the following content:
`cat /flag`

After saving the file, I made it executable with `chmod a+x win`. Then, I ran `export PATH=$PATH:/home/hacker` to add `/home/hacker` to the `PATH` variable and executed `/challenge/run`.

### Hijacking Commands

#### Overriding System Commands
This challenge was tricky but fun. After brainstorming with SENSAI, I came up with the solution:
I opened VSCode again and created a new file called `rm` with the following content:
`cat /flag`

I saved the file and ran `chmod a+x rm` to make it executable. Then, I ran `PATH="~:$PATH"` to add `/home/hacker` to the beginning of the `PATH` so that my custom `rm` would be executed instead of the system's `rm`. Finally, I ran `/challenge/run`.
