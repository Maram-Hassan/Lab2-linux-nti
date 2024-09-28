# Lab2-linux-nti
1.	Change mode of file to give owner read and write permissions and for group write and execute and execute only for the others (using  chmod)
![Screenshot from 2024-09-28 00-51-42](https://github.com/user-attachments/assets/f24bdfc7-7c8a-42fa-adaf-b8069a707f8c)
2.	Change your default permissions to be as above.
![Screenshot from 2024-09-28 00-52-19](https://github.com/user-attachments/assets/61f977bd-1a3d-4bb4-8d9f-ffaf2675782c)

3.	What is the maximum permission a file can have, by default when it is just created? And what is that of directory.
```
file 666
directory 777
```
5.	Change your default permission to read and execute for you (owner), full permission for your group member and no permission for all the others, create a file and a directory. Note the permissions.
![Screenshot from 2024-09-28 01-01-35](https://github.com/user-attachments/assets/4a361770-a2ac-4bb1-be49-ef3daa5e25ae)
![Screenshot from 2024-09-28 01-02-24](https://github.com/user-attachments/assets/4acdfd07-0385-42d4-a36e-d41c93dd383e)
6.	 Copy /etc/passwd to your home directory. Note the permissions allowed to you before and after. Specify why?
![Screenshot from 2024-09-28 14-35-05](https://github.com/user-attachments/assets/0b634b1c-d58b-4b28-b804-66211ef8747a)

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
9.	 Create a file with permission 444. Try to edit in it and to remove it? Note what happened. (notice write protection in LINUX)
```has no write permissions read only ```
![Screenshot from 2024-09-28 14-35-05](https://github.com/user-attachments/assets/9b484edd-1c92-4d77-b0f3-68273e5f7241)
![Screenshot from 2024-09-28 14-37-20](https://github.com/user-attachments/assets/41ff265f-3e7e-42ce-9c66-39dc91ba8913)

What is the difference between the “x” permission of a file and of a directory?
```execute for file means excute script while in directory means access it by cd```

10.	Using the useradd command, add accounts for the following users in your system: user1, user2, user3, user4, user5, user6 and user7. Remember to give each user a password.
![Screenshot from 2024-09-28 15-19-09](https://github.com/user-attachments/assets/ac9ebed2-8c3d-4cab-b4e5-ed62d240bb03)
11.	Using the groupadd command, add the following groups to your system.
Group                      	GID
sales                         	10000
hr                             	10001
web                         	10002
![Screenshot from 2024-09-28 14-47-25](https://github.com/user-attachments/assets/7af9ebe7-7b08-4105-b536-dc97439ef962)

12.	Using the usermod command to add user1 and user2 to the sales auxiliary group, user3 and user4 to the hr auxiliary group. User5 and user6 to web auxiliary group. And add user7 to all auxiliary groups  
![Screenshot from 2024-09-28 15-21-46](https://github.com/user-attachments/assets/5d1c228a-5e9b-4e3a-90d2-3ec74b16d748)

13.	Login as each user and use id command to verify that they are in the appropriate groups. How else might you verify this information?
![Screenshot from 2024-09-28 15-24-16](https://github.com/user-attachments/assets/db3bff4a-97ba-4f3a-8600-e56910206d7a)

14.	Create a directory called /depts with a sales, hr, and web directory within the /depts directory.
![Screenshot from 2024-09-28 14-49-15](https://github.com/user-attachments/assets/8b20f5c3-1da0-452c-883d-a38126b26a1e)

15.	Using the chgrp command, set the group ownership of each directory to the group with the matching name
![Screenshot from 2024-09-28 14-50-25](https://github.com/user-attachments/assets/465646a3-5d96-4118-be2f-d92c7fcaa09a)

16.	Set the permissions on the /depts directory to 755, and each subdirectory to 770
![Screenshot from 2024-09-28 14-51-37](https://github.com/user-attachments/assets/1b36ba4f-be83-42af-b3fd-017247ef0b73)

17.	Set the set-gid bit on each departmental directory
![Screenshot from 2024-09-28 14-52-37](https://github.com/user-attachments/assets/e81271e4-e420-46de-9698-2daf8dbc32ad)

18.	Use the su command to switch to the user2 account and attempt the following commands:
a.	touch /depts/sales/user2.txt
b.	touch /depts/hr/ user2.txt
c.	touch /depts/web/ user2.txt
Which of these commands succeeded and which failed? What is the group ownership of the files that were created?

19.	Configure sudoers file to allow user3 and user4 to use /bin/mount and /bin/umount commands, while allowing user5 only to use fdisk command.
