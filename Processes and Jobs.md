# Listing Processes
`ps aux` or `ps -ef` can be used to list the running processes on the system. Both result in slightly different, but cross-recognizable output.<br>
In this challenge, `/challenge/run` was renamed to some arbitrary command , so I listed the running processes to find the command.<br><br>
![image](https://github.com/user-attachments/assets/081235d2-dd64-4195-9065-a32c4b2a736c)

# Killing Processes
`kill` command can be used to terminate processes.<br>
In this challenge, `/challenge/run` wont start until the `/challenge/dont_run` is terminated, so I listed the running processes to find the PID for `/challenge/dont_run` and terminated the process.<br><br>
![image](https://github.com/user-attachments/assets/36f48797-ab33-4165-a475-2d1ef3f8677e)

# Interrupting Processes
*Ctrl-C* (e.g., holding down the Ctrl key and pressing C) sends an "interrupt" to whatever application is waiting on input from the terminal and, typically, this causes the application to cleanly exit.<br><br>
![image](https://github.com/user-attachments/assets/64340f0c-5857-4789-a9b5-cb31c953c98b)

# Suspending Processes
You can suspend processes to the background with *Ctrl-Z*. This makes the terminal free to use for other processes.<br><br>

![image](https://github.com/user-attachments/assets/6f3fcdc0-6fbb-45f4-a5da-75cbdc894454)

# Resuming Processes
To resume processes, shell provides the `fg` command, a builtin that takes the suspended process, resumes it, and puts it back in the foreground of your terminal.<br><br>

![image](https://github.com/user-attachments/assets/d07388de-70de-478d-91dd-3459673e1865)

# Backgrounding Processes
`fg` is used to resume a process in the foreground. We can also resume a process in the background using `bg`. This will allow the process to keep running, while giving you your shell back to invoke more commands in the meantime.<br><br>

![image](https://github.com/user-attachments/assets/3fa4f85a-2991-4f09-8ece-0ee21b053365)

# Foreground Processes
You can foreground a process which had been backgrounded just by using `fg`.<br><br>

![image](https://github.com/user-attachments/assets/42185839-9888-4561-a4dc-c1ed86228a92)

# Starting Backgrounded processes
You can directly background a process without suspending it by appending `&` with it.<br>
***Syntax***
```
<command> &
```
![image](https://github.com/user-attachments/assets/4780c6cf-e4a6-49d3-b66d-10792d42a870)

# Process Exit Codes
Every shell command, including every program and every builtin, exits with an exit code when it finishes running and terminates. This can be used by the shell, or the user of the shell to check if the process succeeded in its functionality.<br>
You can access the exit code of the most recently-terminated command using the special `?` variable (prepend it with `$` to read its value).<br><br>

![image](https://github.com/user-attachments/assets/a43acf7f-19e1-4d0a-a260-0e94630220ac)

