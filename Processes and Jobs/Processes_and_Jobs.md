### Listing Processes
I executed `ps -ef` in the terminal to view all processes and noticed that `/challenge/29105-run-14038` was running.  
I then ran `/challenge/29105-run-14038`, which successfully provided the desired output.

### Killing Processes
After running `ps -ef` again, I identified the process `/challenge/dont_run` with PID 73.  
I used `kill 73` to terminate that process, then executed `/challenge/run`, which yielded the expected result.

### Interrupting Processes
I ran `/challenge/run` and interrupted the process by hitting `Ctrl+C`. This action resulted in the output I was looking for.

### Suspending Processes
I executed `/challenge/run` and then used `Ctrl+Z` to suspend the process.  
I launched another instance of `/challenge/run` while the first one was suspended and obtained the output I needed.

### Resuming Processes
I suspended a running instance of `/challenge/run` by pressing `Ctrl+Z`.  
Then, I used `fg` in the terminal to resume the suspended process, successfully retrieving the output.

### Backgrounding Processes
I suspended the `/challenge/run` process using `Ctrl+Z` and then used `bg` to move it to the background.  
Afterward, I ran `/challenge/run` again to launch another instance while the first one was still running in the background.

### Foregrounding Processes
When I executed `/challenge/run`, it prompted me to suspend it, then resume in the background, and finally foreground it without resuspending.  
I hit `Ctrl+Z` to suspend the process, followed by `bg` to move it to the background.  
After a bit of scrolling through the terminal output, I used `fg` to bring it back to the foreground, which allowed me to proceed.

### Starting Backgrounded Processes
I ran `/challenge/run &` to start the process in the background, achieving the desired outcome.

### Process Exit Codes
I executed `/challenge/get-code` to retrieve the exit error code of the process.  
Then, I used `/challenge/submit-code $?` to submit the exit error code and successfully completed the task.
