# Cat : not the pet, but the command<br>
Learnt that `cat` is used for reading the contents of a file. It can also concatenate multiple files.<br>
For example:
```
hacker@dojo:~$ cat myfile
This is my file!
hacker@dojo:~$ cat yourfile
This is your file!
hacker@dojo:~$ cat myfile yourfile
This is my file!
This is your file!
```
Used `cat flag` to access the flag <br><br>
![image](https://github.com/user-attachments/assets/38877997-9651-48ff-bbb3-1ef5b6698549)

# catting absolute paths<br>
`cat` can be used to read files outside ***cwd*** by specyfying absolute path of file as `cat`'s arguement.<br><br>
![image](https://github.com/user-attachments/assets/b1c44195-fd31-4d06-a93d-68a8fd9405fc)

# more catting practice <br>
The challenge restricted the use of `cd` command and forced to use the absolute path as arguement of `cat`.<br><br>
![image](https://github.com/user-attachments/assets/58df3d82-fee2-46c7-813c-8f208a1a5ba9)

# grepping for a needle in a haystack<br>
Learnt the use of `grep` to search for specific keywords that in a line of text of a file with a lot of data.<br><br>
![image](https://github.com/user-attachments/assets/e45b54aa-6c42-41c0-b059-0f1a97db0a84)

# listing files<br>
Learnt the use of `ls` which lists the contents of the ***cwd***.<br>
The challenge hid the flag in random file in the `challenge` folder. Used `ls` to find the file.<br><br>
![image](https://github.com/user-attachments/assets/3c0a3908-9469-4adc-96c5-0b00faf2ddf1)<br>
![image](https://github.com/user-attachments/assets/f4b84e55-05d5-4a4c-a677-db3210ce8c76)

# touching files<br>
`touch` is used to create files. The challenge wanted us to create 2 files using `touch`.<br><br>
![image](https://github.com/user-attachments/assets/7b56ebca-f701-4db6-81cb-6e5e5d70b9c3)

# removing files<br>
`rm` is used to remove files. The challenge created a `delete_me` file which was required to be deleted using `rm`.<br><br>
![image](https://github.com/user-attachments/assets/7294d848-d360-429e-807d-9092c275d9df)

# hidden files<br>
Learnt that some files can be hidden from `ls` by simply putting `.` infornt of the filename.<br>
Hidden files can be listed by using  `ls -a`.<br><br>
![image](https://github.com/user-attachments/assets/a612b779-e7fb-4795-942d-c5bd39fad972)

# An epic file system 
The challenge tests the understanding of `cd` , `ls` and `cat` commands. The flag was hidden deep in the system and the flag was to be found by reading the clue files using the forementioned commands.

# making directories
Learnt that `mkdir` can be used to create directories. Challenge specified to make a diretory and create a file in that.<br><br>
![image](https://github.com/user-attachments/assets/9bc172b9-2495-430a-87b0-0208a385b55e)

# finding files 
Learnt that `find` can be used to find directories and files. One can specify location or name of the file to search. The challenge hid the flag somewhere in `/`.<br>
***Command***
```
find / -name flag
```
Found multiple files having name 'flag'. Accessed all of them using `cat` and found out the correct one.<br><br>
![image](https://github.com/user-attachments/assets/a0b7e081-6c82-41e9-a455-68258e7b360a)
