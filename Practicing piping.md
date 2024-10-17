# Redirecting output
`stdout` can be redirected to files by using `>`.<br><br>
![image](https://github.com/user-attachments/assets/c370ca94-7bac-417c-ad6e-cafcc8ddb733)

# Redirecting more output
You can redirect the output of any command using `>`.<br><br>
![image](https://github.com/user-attachments/assets/5d4ffc9a-f4a3-47e0-8f8c-8dd8920e01a0)

# Appending output 
`>>` can be used to append input to a file which already has some data and does not overwrite the existing data.<br><br>
![image](https://github.com/user-attachments/assets/55873fea-af1a-4c81-ac09-dc5dd84b6796)<br><br>

![image](https://github.com/user-attachments/assets/00931749-44bf-4bd1-94de-a93c23d25969)

# Redirecting errors
Got to know about ***file descriptor number*** , the three `fd`s (FD0->input, FD1->output, FD2->error).<br><br>
![image](https://github.com/user-attachments/assets/9dedc48b-5ad7-48a7-a90a-90ead51522be)

# Redirecting input
`<` can be used to redirect input. The file to the right of `<` contains the input which needs to be redirected to the command on the left side of `<`.<br><br>
![image](https://github.com/user-attachments/assets/afde4f8a-9c68-46a3-bf19-2f02bdd87c57)

# Grepping stored results
Used the combination of `>` and `grep` to find the flag.<br><br>
![image](https://github.com/user-attachments/assets/170cd623-b17f-4cd6-8ec1-13d462220877)

# Grepping live output
`|` (pipe operator) has can be used to avoid the need to store results to a file. Standard output from the command to the left of the pipe will be connected to (piped into) the standard input of the command to the right of the pipe.<br><br>
![image](https://github.com/user-attachments/assets/f8edaa39-bd04-4740-a684-245b96a0d80a)

# Grepping errors
Got to know that `>&` can be used to redirect one file descriptor to another. <br><br>
![image](https://github.com/user-attachments/assets/f2f5004d-ed50-4528-943c-bf3dbc063221)

# Duplicating piped data with tee
The `tee` command, named after a "T-splitter" from plumbing pipes, duplicates data flowing through your pipes to any number of files provided on the command line.<br><br>
![image](https://github.com/user-attachments/assets/77d57738-1115-4c51-8307-adcc3b3aa00f)

# Writing to multiple programs
Learnt about the ***Process Substitution*** method which is used to  feed the output of a process (or processes) into the stdin of another process.<br>
***SYNTAX***
```
>(command)
```
![image](https://github.com/user-attachments/assets/4ead0460-72a1-4f68-a9db-9c6b571d4380)

# Split-piping stderr and stdout
![image](https://github.com/user-attachments/assets/116be2ea-9e1c-4a0a-8393-ff6253b5118e)
