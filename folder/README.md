# Folder and Link

#### Find the INode
```sh
ls -il
```
#### Create a soft link or symbolic
```sh
ln -s ${src} ${dest}

```
- -s : create soft link or symbolic link
- src:  Source of the file
- dest: Destination of the file
***
#### Notes
- Inode is different in symbolic link
- Symbolic link can be moved to external HD

#### Create a hard link
```sh
ln ${src} ${dest}
```
- Inode will be same for hard link
- This doesn't need an option
- Hard link is duplicate entry
- Hard link can't be move to external HD
