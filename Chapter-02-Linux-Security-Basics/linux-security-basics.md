Linux Security Basics Lab  
 
Do the following in the terminal of your Virtual Machine (VM). Take screenshots of your commands and output. Explain briefly the purpose of each command as you go. You may organize your lab however you would like. 
General System Tasks: 
1.	Open the terminal in your Virtual Machine (VM). Enter the command to retrieve available updates.
 
 
2.	Upgrade your system.
  
3.	Reboot your system. 
 
User Tasks:  
4.	Change the current user to root using the command sudo su root.  What does the prompt look like? 
  
5.	While logged in as root, create a new user with the name bobby using the command useradd. Next, create another user with the name sally using the command adduser. What is the difference between the two?
  
6.	Change the current user to sally. What does the prompt look like now? 
  
7.	While you’re logged in as sally still, try to create a new user with the name earl. What happens? Why? What could you do to allow her to create a new user? 
 
8.	Enter exit until you are logged into your own account again. Delete the user bobby. I didn’t show you the command, but Google it! Learning how to find information is an important skill in CS; It’s impossible to know everything.  
 
9.	Change the password of sally to something you can remember using sudo passwd sally 
  
10.	Even though it’s easier to complete tasks/commands, why is it bad practice to stay logged in as root?  
Because anyone can log in on your computer and make changes that might be bad for you
11.	Enter the command to see what your user id is. 
 
Group Tasks:  
12.	What groups does ubuntu belong to?  
 
13.	Give sally the ability to execute sudo commands. Next, try to create a new user while logged in as sally. 
  
14.	Log out of Sally and back into your own account. Create a new group called cybersec  
 
15.	Add sally to the group, cybersec  
 
16.	Check to see which groups sally belongs. What are the various ways to do this? 
 
Permission and Access Control Lists: 
17.	Create a new directory called lab1. Enter the command to find the permissions of the directory. Who is the owner and group owner of this directory? What permissions does the owner, group and other have? 
 
18.	Change your directory to lab1. Create a new bash file called, helloWorld. When ran, your program should just print “Hello World!”. (Don’t forget to make your bash file executable).
  
19.	Enter the command ls -l helloWorld. What are the reading, writing, and executing permissions for the owner, group and other? 
 
a.	Change the permissions so the group also has w and x permissions. 
 
20.	Use the getfacl command to view the ACL of the file. 
 
21.	Using the setfacl command, allow the user, sally, the ability to read and write to 
the file. 
  
OPTIONAL — In case you want to learn more: 
The following is a free textbook on learning the Linux command line. It has great reviews, and is an awesome resource if you are interested in learning more: https:// linuxcommand.org/tlcl.php
