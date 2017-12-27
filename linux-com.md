# Linux Use

## check version

```
$ lsb_release -a
$ uname -a
$ uname -r
$ uname -mrs
$ cat /proc/version
$ cat /proc/sys/kernel/{ostype,osrelease,version}
$ cat /etc/*release

```

## First Install

> Update



> install package

```
$ sudo dpkg -i packagename.deb

To remove a Debian (Ubuntu) package (.deb):

$ sudo dpkg -r packagename

To Reconfigure/Repair an installed Debian (Ubuntu) package (.deb):

$ sudo dpkg-reconfigure packagename

apt-get update

apt-get upgrade
```

## User

### Add user

```sh
-- Add user
$ sudo useradd -m <name>
$ cd /home/name 

-- pass
$ sudo passwd <name>
```

### check list user

```
$ cat /etc/passwd

$ awk -F':' '{ print $1}' /etc/passwd
```

### Unzip .tar.xz

```
tar xvfJ filename.tar.xz
```
