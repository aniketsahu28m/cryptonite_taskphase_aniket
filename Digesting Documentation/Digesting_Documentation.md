## Learning from Documentation
I executed the `/challenge/challenge --giveflag` command in the terminal, which successfully provided the flag.

## Learning Complex Usage
I ran the command `/challenge/challenge --printfile /flag` in the terminal, which also successfully retrieved the flag.

## Reading Manuals
I ran the `man challenge` command in the terminal to access the manual for the challenge command.  
In the SYNOPSIS and DESCRIPTION sections, I found the following information:

### NAME
`/challenge/challenge` - Print the flag!

### SYNOPSIS
`challenge OPTION`

### DESCRIPTION
Output the flag when called with the right arguments.

- `--fortune`: Read a fortune.
- `--version`: Output version information and exit.
- `--kkvcpj NUM`: Print the flag if NUM is 838.

I then executed the command `/challenge/challenge --kkvcpj 838` in the terminal, which successfully retrieved the flag.

## Searching Manuals
I executed the `man challenge` command in the terminal to read the manual for the challenge command.  
I used the `/` key to search for "flag" within the manual and discovered the following information in the DESCRIPTION section:

- `--fztkts`: This argument will give you the flag!

After exiting the manual by pressing `q`, I ran the command `/challenge/challenge --fztkts` in the terminal, which successfully retrieved the flag.

## Helpful Programs
I ran the `/challenge/challenge --help` command in the terminal to get assistance with the challenge command.  
Under the optional arguments section, I found the following information:

- `-h, --help`: Show this help message and exit.
- `--fortune`: Read your fortune.
- `-v, --version`: Get the version number.
- `-g GIVE_THE_FLAG, --give-the-flag GIVE_THE_FLAG`: Get the flag, if given the correct value.
- `-p, --print-value`: Print the value that will cause the `-g` option to give you the flag.

I then ran `/challenge/challenge -p` in the terminal to print the value that would work with the `-g` option to retrieve the flag. It provided the value `652`.  
Finally, I executed `/challenge/challenge -g 652` in the terminal and successfully retrieved the flag.

## Help for Builtins

I ran the `help challenge` command in the terminal to learn more about the challenge builtin command. Here's the information I found:

`challenge`: This command will read the flag, given the correct arguments!

#### Options:
- `--fortune`: Display a fortune.
- `--version`: Display the version.
- `--secret VALUE`: Prints the flag if the correct VALUE is provided.

To retrieve the flag, the correct value for `--secret` is "0S9-Bc7U".  
I then executed the command `challenge --secret 0S9-Bc7U` in the terminal and successfully obtained the flag.
