![Shell permission example](https://linuxcommand.org/images/file_permissions.png)
# Shell, permissions

Task 0 **[su betty]** Create a script that switches the current user to the user betty. 

Task 1 **[id -um]** Write a script that prints the efective username of the current user.

Task 2 **[groups]** Write a script that prints all the groups the current user is part of.

Task 3 **[chown betty hello]** Write a script that changes the owner of the file hello to the user betty.

Task 4 **[touch hello]** Write a script that creates an empty file called hello.

Task 5 **[chmod 744 hello]** Write a script that adds execute permission to the owner of the file hello.

Task 6 **[chmod 754 hello]** Write a script that adds execute permission to the owner and the group owner, and read permission to other users, to the file hello.

Task 7 **[chmod a+x hello]** Write a script that adds execution permission to the owner, the group owner and the other users, to the file hello.

Task 8 **[chmod 007 hello]** Write a script that sets the permission to the file hello as follows, Owner: no permission at all, Group: no permission at all, Other users: all the permissions.

Task 9 **[chmod 753 hello]** Write a script that sets the mode of the file hello to this: -rwxr-x-wx

Task 10 **[chmod 354 hello]** Write a script that sets the mode of the file hello the same as olleh’s mode.

Task 11 **[chmod -R a+X .]** Create a script that adds execute permission to all subdirectories of the current directory for the owner, the group owner and all other users. Regular files should not be changed.

Task 12 **[mkdir -m  751 my_dir]** Create a script that creates a directory called my_dir with permissions 751 in the working directory.

Task 13 **[chgrp school hello]** Write a script that changes the group owner to school for the file hello. 

Task 14 **[chown vincent:staff ./*]** Write a script that changes the owner to vincent and the group owner to staff for all the files and directories in the working directory. 

Task 15 **[chown -h  vincent:staff _hello]** Write a script that changes the owner and the group owner of _hello to vincent and staff respectively.

Task 16 **[chown --from=guillaume vincent hello]** Write a script that changes the owner of the file hello to vincent only if it is owned by the user guillaume.
