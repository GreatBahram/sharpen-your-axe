# Shell Job Control

Link to the main article: [Link](https://jvns.ca/blog/2024/07/03/reasons-to-use-job-control/)

## Process States in Terminal

- **Foreground**: The process is actively running and taking input from the terminal.
- **Background**: The process runs in the background, allowing you to continue using the terminal. Example: `my_app &`
- **Stopped**: The process is temporarily halted. This occurs when you press `Ctrl + z`.

## how to use job control

- `fg`: Brings a process to the foreground.

- `bg`: Restarts a stopped process and puts it in the background.

- `Ctrl + z`: Stops the current foreground process.

- `jobs`: Lists all processes that are active in your terminal.

- `kill`: Sends a signal (like `SIGKILL`) to a job to terminate it.

- `disown`:  Removes the job from the list of running jobs, so that it doesn’t get killed when you close the terminal.
- `nohup`: Keeps a process running even after you log out or close the terminal and it redirects the output to a file (usually `nohup.out`)