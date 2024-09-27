# Lab2-linux-nti
1.	Change mode of file to give owner read and write permissions and for group write and execute and execute only for the others (using  chmod)
![Screenshot from 2024-09-28 00-51-42](https://github.com/user-attachments/assets/f24bdfc7-7c8a-42fa-adaf-b8069a707f8c)
2.	Change your default permissions to be as above.
![Screenshot from 2024-09-28 00-52-19](https://github.com/user-attachments/assets/61f977bd-1a3d-4bb4-8d9f-ffaf2675782c)

3.	What is the maximum permission a file can have, by default when it is just created? And what is that of directory.
file 666
directory 777

5.	Change your default permission to read and execute for you (owner), full permission for your group member and no permission for all the others, create a file and a directory. Note the permissions.
![Screenshot from 2024-09-28 01-01-35](https://github.com/user-attachments/assets/4a361770-a2ac-4bb1-be49-ef3daa5e25ae)
![Screenshot from 2024-09-28 01-02-24](https://github.com/user-attachments/assets/4acdfd07-0385-42d4-a36e-d41c93dd383e)
6.	 Copy /etc/passwd to your home directory. Note the permissions allowed to you before and after. Specify why?

7.	What are the minimum permission needed for :
a.	Copy a directory  (source and target)
     rwx
b.	Copy a file (source and target)
     rw
c.	Delete  a file
      w
d.	change  to a directory
      x
e.	List a directory content
      rx
f.	  View a file content
      r
g.	Modify a file content
      w
8.	 Create a file with permission 444. Try to edit in it and to remove it? Note what happened. (notice write protection in LINUX)
What is the difference between the “x” permission of a file and of a directory?
9.	Using the useradd command, add accounts for the following users in your system: user1, user2, user3, user4, user5, user6 and user7. Remember to give each user a password.

10.	Using the groupadd command, add the following groups to your system.
Group                      	GID
sales                         	10000
hr                             	10001
web                         	10002

11.	Using the usermod command to add user1 and user2 to the sales auxiliary group, user3 and user4 to the hr auxiliary group. User5 and user6 to web auxiliary group. And add user7 to all auxiliary groups  

12.	Login as each user and use id command to verify that they are in the appropriate groups. How else might you verify this information?

13.	Create a directory called /depts with a sales, hr, and web directory within the /depts directory.

14.	Using the chgrp command, set the group ownership of each directory to the group with the matching name

15.	Set the permissions on the /depts directory to 755, and each subdirectory to 770

16.	Set the set-gid bit on each departmental directory

17.	Use the su command to switch to the user2 account and attempt the following commands:
a.	touch /depts/sales/user2.txt
b.	touch /depts/hr/ user2.txt
c.	touch /depts/web/ user2.txt
Which of these commands succeeded and which failed? What is the group ownership of the files that were created?

18.	Configure sudoers file to allow user3 and user4 to use /bin/mount and /bin/umount commands, while allowing user5 only to use fdisk command.
