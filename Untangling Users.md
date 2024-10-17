# Becoming root with su
Becoming root is a fairly common action that Linux users take, therefore there are two utilities used for this purposes: `su` and `sudo`.<br>
But `su` is an old method to elevate the user to root access. It checks for root password.<br><br>
![image](https://github.com/user-attachments/assets/209cb770-d536-4a6b-9fbf-9fbc11bab51f)

# Other users with su
You can give any username as an arguement to `su` to switch to that user instead of root.<br><br>
![image](https://github.com/user-attachments/assets/2c54cebd-c2b9-4815-8b0e-25aa0358f889)

# Cracking passwords
Learnt the use of the famous program ***John The Ripper***. 
***Syntax**
```
john <passwd-file>
```
Used this command to crack the password of user 'Zardus'.<br><br>
![image](https://github.com/user-attachments/assets/5bc353dd-22eb-46b6-b9ff-eb28f953f4f1)

# Using sudo
`sudo` defaults to running a command as root. `sudo` relies on policies that it checks to determine the user's authorization run things as root. These policies are defined in /etc/sudoers.<br><br>
![image](https://github.com/user-attachments/assets/d91787c8-5a30-43d7-9ac7-221d27fdbe5e)
