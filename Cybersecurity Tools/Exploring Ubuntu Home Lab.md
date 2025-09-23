# Exploring Ubuntu Home Lab

---

Before beginning:
1) Ran 'sudo apt update' to refresh my package index and show my system which packages could be updated.
2) Ran 'sudo apt upgrade' to install any updates my system needed.
3) Ran 'sudo reboot' to guarantee the system applied all updates consistently.

Lab:
4)
![Switch to Root User Command](../images/l1q4.png)

I switched to the root user, which can differentiated by the # at the end of the line rather than a $. It is also root@ instead of delamaterk@.

5)
![useradd and adduser commands](../images/l1q5.png)

The useradd command only creates the user, while adduser uses a perl script to create a password and home directory for the user. As you can see, I had trouble with setting the password because I though bad password meant I had to do a different password.

![Switching to user sally](../images/l1q6.png)

6) Using the 'su' command, I switched to the user sally I created in the previous step. Now, the prompt has sally@ instead of root@ and has switched from # back to $. 

![Trying to create new users as sally](../images/l1q7.png)

7) I tried to add a new user named earl while I was sally, which it did not allow me to do because the user is not the root user/does not have sudo privileges.

![Returning to ubuntu user](../images/l1q8.png)

8) I used the exit command twice to return to my user 'delamaterk'. Then, I did 'userdel earl' to ensure the user was not created by sally.

![Changig sally's password](../images/l1q9.png)

9) I was able to change sally's password using 'sudo passwd sally' because I have sudo privileges.

10) For the rest of my tasks I will stay logged in as my user because it is bad practice to stay logged in as root. Running commands as the root user reduces security, can easily damage the system, and there is little accountability for any actions.

![Checking my id](../images/l1q11.png)

11) Using the 'id' command, I can see that my user id is 1000.







