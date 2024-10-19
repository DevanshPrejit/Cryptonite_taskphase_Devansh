# The PATH Variable
There is a special shell variable, called PATH, that stores a bunch of directory paths in which the shell will search for programs corresponding to commands.<br>
If the PATH variable is set to an empty string, many programs will malfunction (some might not if they are builtins). <br>
To complete this challenge, I set the PATH variable empty to malfunction the `rm` command that deletes the flag.<br><br>
![image](https://github.com/user-attachments/assets/2edbe6f5-58e0-4a35-bb74-f17328d9de3f)

# Setting PATH
There is a method to execute programs wihtout using their absolute paths. You can just overwrite the PATH variable with the directory in which your program exists.<br>
For this you need to do the following :<br>
```
PATH="program-directory"
```
Now you can run the program by its bare name.<br><br>
![image](https://github.com/user-attachments/assets/b814cca1-de3a-4d7c-96ff-31e8400d10dc)

# Adding Commands
There is a way make our own commands and use them just by their bare names. This can be done by making a shell script for the command, making it executable and then adding the directory of the shell script to the PATH variable.<br><br>
![image](https://github.com/user-attachments/assets/80ecff97-2dc4-4148-99ef-d327c7ca533c)

# Hijacking Commands
In this challenge, running `/challenge/run` executes `rm` command in the flag. Emptying the PATH variable doesn't give the flag, so we overwrite the `rm` command with `cat /flag` and trick it into opening the flag!<br><br>
![image](https://github.com/user-attachments/assets/3435457c-942b-47e4-a2c4-23616637cb35)
