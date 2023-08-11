# Common

#### Check for previous command status code
```sh
echo $?
```
- 0  : Success
- 1 : Failure

#### Run previous command again
```sh
!!
```
#### Create a file
```sh
touch -m ${file}
```
- -m : Change the DateTime of the file
#### Show all path variable
```sh
$PATH
```
#### Show content of file
```sh
cat ${file}
```
#### Install Sudo
```sh
apt install sudo
```
####  Check group for the sudo
```sh
cat /etc/sudoers
```
####  Add User to sudo group
```sh
usermod -aG sudo ${user}
```
```sh
sudo -l
```


#### less, tail, head, echo, man, find, inode, touch, wc, wget