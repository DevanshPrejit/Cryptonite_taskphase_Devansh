# Printing Variables
Learnt how the value of any variable can be printed using `echo`.<br><br>
![image](https://github.com/user-attachments/assets/baadef25-827f-454e-9405-0e764ffeb6d3)

# Setting Variables 
Variable can be assigned a value using `=`. <br>
For example : STR='Hello', where STR is a variable and ***Hello*** is a value stored in it.<br><br>
![image](https://github.com/user-attachments/assets/0193a6b9-3430-4df3-9e4a-840bf3652d52)

# Multi-word variables 
*Quoting* can be used to assign values having space between them.<br><br>
![image](https://github.com/user-attachments/assets/218e5b50-4174-4754-86a6-0590514dbbde)

# Exporting variables
Variables assigned in one shell cannot be used in the other shell. For this you need to explicitly ***export*** it using the command `export <variable>`.<br><br>
![image](https://github.com/user-attachments/assets/b0e1d516-5d8c-4f70-884d-6f5a1635fc0f)

# Printing exported variables
`env` can be used to printout the value of an exported value.<br>
Syntax-
```
env $<variable_name>
```
![image](https://github.com/user-attachments/assets/4cc2e454-3f39-45f0-923f-dc79840c9af8)

# Storing command output
You can store output of any command to a variable using `$()`.<br><br>
![image](https://github.com/user-attachments/assets/c6d615dd-87cb-4da8-a85b-5e50e4444d7d)

# Reading input
`read` can be used to input any value from the user and assign it to a variable.<br><br>
![image](https://github.com/user-attachments/assets/5c52802a-76c3-4548-bcc2-36f12cbaf707)

# Reading files 
We can redirect the output of any program as an input to the `read <variable>` command using `<`.<br><br>
![image](https://github.com/user-attachments/assets/4d1fe9b9-3ee8-4895-a376-ec106f872da4)
