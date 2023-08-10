# User and Group

#### Check all the User
```sh
cat /etc/passwd
```
#### List the current User
```sh
whoami
```
#### Add a User
```sh
useradd -m vimal
```
- -m (Optional): will create folder home dir
- -r (Optional): will create system user
#### Delete a User
```sh
userdel -r vimal
```
- -r (Optional): will delete home dir

### Add Password
```sh
passwd
```
- Can give the user as arguments

### View hashed password file
```sh
cat etc/shadow
```

### Show groups
```sh
groups
```
- Can give the user as arguments

#### Check all the Group
```sh
cat /etc/group
```
