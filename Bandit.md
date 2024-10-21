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
# 
