# The Root <br>
Learnt that all filesystems start with `/` which is used to access the directories, files and programs in a system.<br>
Invoked `/pwn` to access the flag.<br>
***Output***<br><br>
![image](https://github.com/user-attachments/assets/63800a2a-6130-4703-b489-6c15445de506)

# Program and Absolute paths<br>
Learnt to access programs using its *absolute path* .<br>
Executed `/challenge/pwn` to get the flag.<br><br>
![image](https://github.com/user-attachments/assets/ddead165-fa30-4a88-90c8-f6c397ea74ac)

# Position Thy Self<br>
Learnt that `cd` is used to change the current working directory. Also came to know what `~` signifies (shorthand for home directory).<br>
***Command used to access flag***<br>
```
cd /usr/share/build-essential 
/challenge/run
```
***Output***<br><br>
![image](https://github.com/user-attachments/assets/a6ceb5f2-6c45-430c-ad30-67573ad456e2)

# Position elsewhere <br>
Used different directory to access the flag.<br>
Committed mistake while opening directory <br><br>
![image](https://github.com/user-attachments/assets/7f8b27e3-c5e9-454f-ba3a-ae3974519bb4)<br><br>
Corrected the mistake and got the flag.<br><br>
![image](https://github.com/user-attachments/assets/d497ebb2-860d-4dee-96af-32d36052b3a6)

# Position yet elsewhere 
Used `cd` to access flag.<br><br>
![image](https://github.com/user-attachments/assets/694f902e-5f47-4c53-98d3-1f2635554be4)

# Implicit relative paths, from '/'<br>
Learnt about **relative paths** which can be used to access programs within the `cwd`.<br>
Committed mistake by using absolute path of program.<br><br>
![image](https://github.com/user-attachments/assets/6a6590d4-ea92-49a6-a798-4dc7cf4b689c)<br><br>
Used relative flag to access the flag<br><br>
![image](https://github.com/user-attachments/assets/bf3a3e7c-777b-4506-8644-e0f8b0384780)

# Explicit relative paths, from '/'<br>
Learnt that `.` symbol in a path represents the current directory.<br>
This means that when you use `./` before a directory or file name, you're explicitly stating that you're referring to something in the current directory.<br>
For example, if you're in the /challenge directory and you want to refer to a file named example.txt, you could use:<br>
`example.txt` (implicitly in the current directory)<br>
`./example.txt` (explicitly in the current directory)<br>
Both paths point to the same file, but the second one uses `.` to make it clear that the file is in the current directory.

# Implicit relative path 
Learnt that Linux explicitly avoids automatically looking in the current directory when you provide a "naked" path.<br><br>
![image](https://github.com/user-attachments/assets/bad14326-13c8-46e5-a025-a366f104acdb)

# home sweet home
Learnt how pass a file as an arguement.<br>
Deeply understood the use of `~`.<br><br>
![image](https://github.com/user-attachments/assets/65620d30-74ed-4a02-8a1c-3ebb8bdc23ca)
