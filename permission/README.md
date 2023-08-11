# Permission
listing all the fils and folder 
```sh
ls -l
```
Output to look like this
```sh
drwxr-xr-x   2 root root 4096 Apr 18  2022 boot
lrwxrwxrwx   1 root root    7 Jun 24 02:02 lib -> usr/lib
-rwxr-xr-x   1 root root    0 Aug 10 22:18 .dockerenv
```
BreakDown
```sh
rwx
```
- r (4): Read Permission
- w (2): Write Permission
- x (1): execute

Breakdown 
```sh
drwxr-xr-x   2 root root 4096 Apr 18  2022 boot
```
- d   : Represent directory
- rwx : Permission for user 
- r-x : Permission for group
- r-x : Permission for other

Add Permission
```sh
chmod u+xrw ${file}
```
- +x : Will add execute command to all
- -x : Will remove execute command to all
- u+x: Will add execute command to User
- g+x: Will add execute command to Group
- O+x: Will add execute command to Other
- -R : Will recursive add permission

Add Permission with numbers
```sh
chmod 770 ${file}
```
Change the Ownership
```sh
chown ${user}:${group} ./folder
```
- user (Optional): User to change to
- group (Optional): Group to change to
