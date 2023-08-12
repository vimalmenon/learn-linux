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
####  Display what is allowed to be done
```sh
sudo -l
```
### Allows to edit sudoers file
```sh
sudo visudo
```

#### Sequence of number
```sh
seq 5
```

## xargs
```sh
ls |xargs ls
```
- -I : Give the variable to use
- -t : Give what command 
- -n : Number of arguments
- -p : Number of processes
#### Time any command (Show how much time to took to execute)
```sh
time ${command}
```
## awk
```sh
cat /etc/passwd | awk -F ":" '{print $2}'
```
- -F : delimiter to use

```sh
cat /etc/passwd|awk -F ":" '{print $1 " / "  $3}'
```
#### With regular expression to check
```sh
cat /etc/passwd|awk -F ":" '/^b/ {print $1}'
```
#### Checking if condition
```sh
ps |awk '{ if($1 != "PID") print $0}'
```

## cut
```sh
cut -c 1-5
```
```sh
ps | cut -c 5-
```
- -c : Cut the charters
- -d : Delimiter to use


## tr
##### Replace the character
```sh
ps | tr 'p' 'P'
```
```sh
ps | tr -d 'p'  
```
- -s: Squeal
- -d: Delimiter

### Sed
```sh

```
#### less, tail, head, echo, man, find, inode, touch, wc, wget