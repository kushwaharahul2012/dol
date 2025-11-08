User vs Group vs Others → who owns what.
in text of user its a identity to access project mangment to any file or folder based on user they perform task in our teritory vs in term of group are just a numbers of many resources users or it can be managing also group lavels of things example if a user is assighn a docker group then user can have access right to use docker resources and others mean that user is not the owner (Who created) and group is not the part of this access so all others users comes if they not belong of users or groups come to others section.

What a UID/GID is (show from /etc/passwd if you’re on Linux).
Uid stand For User Identifier Its start with root addministrator 0 uid and normal user 1000-60000 in range its uniqe number assighn to every user and GID group indentifier in default some group also created 1000 Identifies UID so both are define ownership to access those file or resources. in term of /etc/passwd every user details such user password is define in this folder.

File modes: r (read), w (write), x (execute) and how the chmod octal math works (r=4, w=2, x=1).

file mode have define which user or file have access or which types of access have there 3 types of r (read) , w (write), x(excute) each file have that short of access things for every users or group - in chmod octal define access 4 read 2 write and 1 excute and 0 or - is no permission example -rwxr-xr-- 1 alice developers 2048 Oct 15 10:30 script.sh lets look this - its define type here its a file so - if its this folder so here d rwx thats belong to owner here read write and excute permission have
then r-x its permission for group here read and excute permission not w write permission have to group last r-- others in last others have only read permission.

sudo philosophy — least privilege, not “type sudo everywhere.”
sudo is give more addministrator power to users for performing task such as installing or updating or permission related its privilage of root users so you not use sudo when this is not required its basicaly giving rights of freedom to permission mainly sudo use for performing instalation or permission in administrial lavel

What umask does and how it affects default permissions.

umask user file creation masked its comes default for managing permission tho newly created files or group in default every group have 777 permission or file 666 , for newly creted file or group have full permissions because they can perform with full access. umask 022 (Common default on many systems) its comanny used.
