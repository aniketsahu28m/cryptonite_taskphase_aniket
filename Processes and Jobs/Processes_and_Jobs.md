Processes and Jobs
Listing Processes
Ran ps -ef in the terminal to list all active processes and their details.
Noticed the process /challenge/29105-run-14038 running. Executed /challenge/29105-run-14038 in the terminal to see the result.
Killing Processes
Executed ps -ef to list all processes.
Found a process named /challenge/dont_run with PID 73.
Used kill 73 to terminate the process.
Then ran /challenge/run to proceed.
Interrupting Processes
Started /challenge/run in the terminal, and used Ctrl+C to interrupt the running process.
Suspending Processes
Ran /challenge/run and hit Ctrl+Z to suspend the process.
Launched another instance of /challenge/run while the first process was still suspended.
Resuming Processes
Suspended /challenge/run with Ctrl+Z, then resumed the process using the fg command.
Backgrounding Processes
After suspending /challenge/run with Ctrl+Z, used bg to continue the process in the background.
Then started another instance of /challenge/run.
Foregrounding Processes
Executed /challenge/run, which prompted instructions to suspend the process, resume it in the background, and then bring it to the foreground without suspending it again.
Suspended the process with Ctrl+Z, resumed it with bg, and finally brought it to the foreground with fg.
Starting Backgrounded Processes
Used /challenge/run & to start the process directly in the background.
Process Exit Codes
Ran /challenge/get-code to retrieve the process exit code.
Submitted the exit code using /challenge/submit-code $?.
