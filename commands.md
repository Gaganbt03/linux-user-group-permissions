# Linux User, Group and File Permission Management

This document contains all the Linux commands used to create users, groups,
assign users to groups, create files, set permissions, and verify ownership.
This project demonstrates hands-on experience with the Linux Command Line Interface (CLI).

---
# 1. Creating Directory and Changing the Directory
```bash
mkdir google
cd google

# 2. Creating Users
sudo useradd -m Bharath_kumar_m
sudo useradd -m Anil_L
sudo useradd -m Manoj_SK
sudo useradd -m Sanath_S
sudo useradd -m Hemanth_M
sudo useradd -m Karthik_GR
sudo useradd -m Vijay_DR
sudo useradd -m Prajwal_Kumar

# 3. Creating Groups
sudo groupadd Full_Stack_Developer
sudo groupadd Ai_Engineer
sudo groupadd DevOps_Engineer
sudo groupadd Cloud_Engineer
sudo groupadd Cybersecurity_Engineer

# 4. Adding Users to Groups
sudo gpasswd -M Bharath_kumar_m,Anil_L Full_Stack_Developer
sudo gpasswd -M Manoj_SK,Sanath_S Ai_Engineer
sudo gpasswd -M Hemanth_M,Karthik_GR Cloud_Engineer
sudo gpasswd -M Vijay_DR,Prajwal_Kumar Cybersecurity_Engineer
sudo gpasswd -M gagan DevOps_Engineer

# 5. Creating Files
touch full_stack.log
touch ai.log
touch devops.log
touch cloud.log
touch cyber.txt

# 6. Changing File Permissions
chmod 775 ai.log
chmod 775 cloud.log
chmod 775 devops.log
chmod 775 full_stack.log
chmod 775 cyber.txt

# 7. Assigning Files to Specific Groups
sudo chgrp Ai_Engineer ai.log
sudo chgrp Full_Stack_Developer full_stack.log
sudo chgrp DevOps_Engineer devops.log
sudo chgrp Cloud_Engineer cloud.log
sudo chgrp Cybersecurity_Engineer cyber.txt

# 8. Testing and Verification
cat /etc/group
ls -l
```
---

Command Explanation:

1. mkdir google – Creates a new directory.

2. cd google – Moves into the directory.

3. useradd -m username – Creates a user with a home directory.

4. groupadd groupname – Creates a new group.

5. gpasswd -M users group – Adds users to a group.

6. touch filename – Creates an empty file.

7. chmod 775 file – Gives full access to owner & group, read to others.

8. chgrp group file – Assigns file to a specific group.

9. cat /etc/group – Displays groups and members.

10. ls -l – Shows file permissions and ownership.
---
Conclusion:
   This project demonstrates Linux user, group, and permission management using CLI commands.






