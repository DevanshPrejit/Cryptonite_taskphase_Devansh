# Chaining with Semicolons
`;` separates commands in a similar way to how Enter separates lines. Basically, when you hit Enter, your shell executes your typed command and, after that command terminates, give you the prompt to input another command. The semicolon is analogous, just without the prompt and with you entering both commands before anything is executed.<br><br>
![image](https://github.com/user-attachments/assets/36677087-caa4-4deb-a1b7-e244060ac2fd)

# Chaining Commands
### Learnt a new way to run complex consecutive commands in shell.<br>
***Step-1:***
Write the commands in a text editor.<br><br>
![image](https://github.com/user-attachments/assets/b1e965f6-8a65-49c9-a7d4-cb83526852db)<br><br>

***Step-2:*** 
Save the file as `<file-name>.sh`.<br><br>

***Step-3:***
Use the `bash` command and pass the file as an arguement for it.<br><br>
![image](https://github.com/user-attachments/assets/091b0a0a-3b42-46e7-a26c-3741d82667f7)

# Redirecting Script output
We know that `|` is used between one command's output and a different command's input.
Therefore we can send the output of several programs to one command by using `|`.<br><br>
![image](https://github.com/user-attachments/assets/b1e965f6-8a65-49c9-a7d4-cb83526852db)<br><br>
![image](https://github.com/user-attachments/assets/b2767f93-6572-4ad6-9a45-9cea26707fd3)

# Executable Shell scripts
We can run the script directly without using `bash` by making the script file executable using `chmod`.<br><br>
![image](https://github.com/user-attachments/assets/cdad458e-803d-48d7-b9f9-8d0aa7c30974)
