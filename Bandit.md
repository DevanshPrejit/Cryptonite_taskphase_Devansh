# Level 0
Used the command `ssh bandit0@bandit.labs.overthewire.org -p 2220` and pass : **bandit0** to login to SSH.
# Level 0->1
 - Next password was given in ***readme***.
 - used `cat readme` to access the password.
 - used `ssh bandit1@bandit.labs.overthewire.org -p 2220` with the pass: **ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If** 
# Level 1->2
 - next pass was given in `-` file which is a *dashed file* .
 - there are 2 ways to open a *dashed file* : `cat < -` or `cat ./-`
 - used `ssh bandit2@bandit.labs.overthewire.org -p 2220` with pass: **263JGJPfgU6LtdEvgfWU1XP5yac29mFx**
# Level 2->3
 - next pass given in file named ***spaces in this filename***.
 - file which has spaces in it's name can be opened by putting the name in double quotes `" "`.
 - used `ssh bandit3@bandit.labs.overthewire.org -p 2220` with pass: **MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx**
# Level 3->4
 - next pass given in a hidden file.
 - Hidden files have `.` in fornt of their names and can be seen by `ls -a`.
 - used `ssh bandit4@bandit.labs.overthewire.org -p 2220` with pass: **2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ**
# Level 4->5
 - next pass given in file named ***-file07***.
 - this file can be accessed using the same command which was used in **LEVEL-1** which is `cat ./-file07`.
 - used ssh bandit5@bandit.labs.overthewire.org -p 2220` with pass: **4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw**
# Level 5->6
 - next pass hidden in a file, in a subdirectory of `inhere` directory.
 - Since filesize was a unique identifier used the **find** command to locate the file.
   ```
   find /path/to/search -size [+-]N[cwbkMG]
   ```
   ![image](https://github.com/user-attachments/assets/100e202f-9e21-4750-9693-e036db47d8c5)
 - used `ssh bandit6@bandit.labs.overthewire.org -p 2220` with pass: **HWasnPhtq9AVKe0dmk45nxy20cvUa6EG**
# Level 6->7
 - next pass hidden in the server.
 - we know the owner user, owner grp and size so we use find with specified arguements.
   ```
   find / -size 33c -user bandit7 -group bandit6
   ```
 - found the file<br>
 ![image](https://github.com/user-attachments/assets/72cc820a-f4a2-4741-b44e-759a05d99132)
 - used `ssh bandit7@bandit.labs.overthewire.org -p 2220` with pass: **morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj**
# Level 7->8
 - next pass hidden in file ***data.txt*** which was next to the word **millionth**.
 - used piping to find the word **millionth**<br>
 ![image](https://github.com/user-attachments/assets/8c5a1b1e-15d1-4d13-995c-ef004bc5af2f)
 - used `ssh bandit8@bandit.labs.overthewire.org -p 2220` with pass: **dfwvzFQi4mU0wfNbFOe9RoWskMLg7eEc**
# Level 8->9
 - next pass jumbled along with lot of other garbage stuff and is the only line of text that occurs only once, so I used `uniq`.
 - The uniq -u command in Linux is used to display only unique lines from a file or input, but it works only on adjacent duplicate lines. Therefore, to ensure that all duplicates are grouped together, the input must be sorted before using uniq -u.
 - ![image](https://github.com/user-attachments/assets/7b854b1d-4113-449a-a0e4-fa55fc4fbb2a)
 - used `ssh bandit9@bandit.labs.overthewire.org -p 2220` with pass: **4CKMh1JI91bUIZZPXDqGanal4xvAg0JM**
# Level 9->10
 - next pass hidden in file ***data.txt*** which is the only human-readable string, and is preceded by `=`.
 - human-readable data can be filtered out by using `strings <file>`.
 - to find strings preceded by `=`, we can use `grep`.
 - ![image](https://github.com/user-attachments/assets/d8af7af0-2109-4462-bae0-f47b33f279dc)
 -  used `ssh bandit10@bandit.labs.overthewire.org -p 2220` with pass: **FGUW5ilLVJrxX9kMYMmlN4MgbpfMiqey**
# Level 10->11
 - next pass was encoded in ***Base64***.
 - used ***Base64*** decoder to crack the password.
 - ![image](https://github.com/user-attachments/assets/b1875b72-21b7-4c63-b49e-509c611ed17a)
 -  used `ssh bandit11@bandit.labs.overthewire.org -p 2220` with pass: **dtR173fZKb0RRsDFSGsg2RWnpNVj3qRr**
# Level 11->12
 - next pass was encoded in **ROT13**
 - used **ROT13** decoder to crack the password.
 - ![image](https://github.com/user-attachments/assets/c530aa72-3568-42f3-b4a0-91549897abea)
 - used `ssh bandit12@bandit.labs.overthewire.org -p 2220` with pass: **7x16WNeHIi5YkIhWsfFIqoognUTyj9Q4**
# Level 12->13
 - The password for the next level is stored in the file data.txt, which is a hexdump of a file that has been repeatedly compressed.
 - Made a temp directory using `mktemp -d` and copied data.txt to it.
 - used `mv <original-name> <final-name>` to rename the file.<br><br>
 ![image](https://github.com/user-attachments/assets/4556787e-3b5d-4792-a706-368acd8c0edf)
 - Since the file was a hexdump, so I used `xxd -r <file>` to reverse the hexdump and get the original file.
 - Then used `file` to find the type in which the file was compressed.<br><br>
 ![image](https://github.com/user-attachments/assets/3818172e-a5c1-4374-93d1-cd9b097cea47)
 - file was compressed by `gzip`. Changed the file extension to `.gz` and decompressed it using `gzip -d <file>`.<br><br>
 ![image](https://github.com/user-attachments/assets/86d33002-ca49-4a6f-80e7-dba1254cf3b8)
 - used `file` to check the compression type again. Found out it was `bzip2` compressed.
 - repeated the same process as for `gzip`.
 - next file was a `tar` archived file. Used `tar -xf <file>` to extract the files.<br><br>
 ![image](https://github.com/user-attachments/assets/f093e243-b7ed-41dd-8bef-229c8db16b54)
 - `bata5.bin` was again a `tar` file, so i repeated the process.
 - Continued the previous steps to finally get the password.
 - used `ssh bandit13@bandit.labs.overthewire.org -p 2220` with pass: **FO5dwFsc0cbaIiH0h8J2eUks2vdTDwAn**
# Level 13->14
 - 



