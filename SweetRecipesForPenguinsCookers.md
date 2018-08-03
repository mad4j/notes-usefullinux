# Sweet Recipes for Peguin Cookers
aka Quick Hacks for Linux Administrators

## System general information

```
$ uname -a                              # system description
$ uptime                                # how long from last boot
$ hostname                              # system host name
$ hostname -I                           # host IP address
```

## Hardware information
```
$ dmesg                                 # boot and drivers messages
$ lsdev                                 # information on installed hw

$ cat /proc/cpuinfo                     # CPU model and features
$ cat /proc/meminfo                     # HW memory
$ grep MemTotal /proc/meminfo           # installed physical memory
$ free -m                               # free (and occupied) memory in MB (-m)
$ watch -n1 'cat /proc/interrupts'      # watch interrupts every seconds (-n1)
```

## Editing

### VI
When nano or pico are not available.

### Command Mode
The command mode is accessed with [ESC], the insertion mode with *i*.
Use the command *:help* to get information.

#### Quitting
```
:w newfilename                          save the file to newfilename
:wq or :x                               save and quit
:q!                                     quit without saving
```

#### Search and Mode
```
/string                                 search forward for string
?string                                 search backward for string
n                                       search for next instance of string
N                                       search for previous instance of string
1G                                      move to the first line of the file
nG                                      move to the nth line of the file
G                                       move to the last line of the file
:%s/OLD/NEW/g                           search and replave every occurrence of OLD with NEw
```

#### Delete, Copy, Paste
```
dd                                      delete current line
u                                       undo last modification
```

## Autotools Cross-Compilation
It is possible to use standard configure script in order to cross-build an open-source library/application.

```
./configure --host=x86 --target=armv5 --prefix=/tmp/install 
    CC=arm-none-linux-gnueabi-gcc CXX=arm-none-linux-gnueabi-g++

make

make install
```

Supposing:
* host environment Linux on x86
* target architecture ARM processor
* ARM cross-compiler installed and available on PATH
* local installation in /tmp/install folder

# Back in one sigle step
Using **cd -** is possible to return to the previous folder with a single generic command.

```
$ pwd
/home/user

$ cd /etc/dpkg

$ cd -

$ pwd
/home/user
```

## Continuosly watch

```
$ watch -s -n 1 ifconfig eth0
```

## Open the serial port
```
$ microcom -s 115200 /dev/ttyS1
```

## Customize environment

/etc/bash.bashrc
 ~/.bashrc 
 
~/.profile



* watch
* pidstat
* chrt
* time
* sudo !!
* tar
* du
