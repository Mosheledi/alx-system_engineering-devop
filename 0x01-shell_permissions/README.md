su-changes current user to desired user
whoami-tells current user
groups-check all groups current user is a part of
sudo chown-changes file ownwership to desired user
touch hello-creates an empty file called 'hello'
chomd u+rwx,g+r,o+r-adds execute permission to owner of desired file
chmod u+rwx,g+rx,o+r-gives owner and group execute permission but everyone else the read permission
chmod 751-adds execution permission to the owner, the group owner and the other users, to the file hello
chmod 007-sets the permission to the file hello as follows:
Owner: no permission at all
Group: no permission at all
Other users: all the permissions
chmod 753-changes permission for hello file to -rwxr-x-wx
chgrp school hello-changes the group owner to school for the file hello
chmod --reference=olleh hello-mirrors olleh permissions to hello
sudo find Example -type d -exec chmod 755 {} \
umask 751 , mkdir my_dir-creates a directory named my_dir with the specific permissions
