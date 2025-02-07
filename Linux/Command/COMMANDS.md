## Linux Command Cheat Sheet

### Resource:
[Linux & Docker Fundamentals](https://www.youtube.com/watch?v=EUu1E_YKGTw&t=6010s&ab_channel=Kubesimplify)

### Stuck Somewhere?

- `man` - If you get stuck anywhere use this `man<space>command` where you can access the manual of the particualar command! 

### What is OS info?

- OS info is a general term that refers to information about the operating system (OS) running on a computer

### Commands to get info about OS:

- `lsb_release -a`
-  `cat /etc/os-release`
- `uname -a`
- `lscpu`
- `lsmem`

### What is syslog?

- Syslog is a standard protocol used for collecting and storing log messages generated by various system components, applications, and network devices.

### Commands to get info about Syslog:

- `find / -name 'syslog'`
- `cd /var/log` -> `cat syslog` -> `cat syslog | less` (this is used for better representation of logs).

### What is creating a new user in linux?

- Creating a new user in Linux involves setting up a unique account for a specific individual to access the system.

### Commands to create a New User:

- `useradd -D` - This command tell us the information which is defaut for all users.
- `useradd -m <space> username` - This command will create a new user.
- `passwd <space> username` - This command will help you to setup password to the particular user.
-`usermod -aG sudo username` - This command will add your particual user to  sudo group which will help you to run command as root user.
- `su - username` - This command will switch to the particular username.

### What are groups in linux?

- Groups in Linux are essentially collections of users. They're a fundamental part of the operating system's permission structure, making it easier to manage access to files and system resources.

### Commands to play around groups:

- `groupadd <space> groupname` - This  command will help you to create a new group.
- `getent group groupname` - This command will help you to get information of that particualar group.
- `sudo -aG groupname $USER` - This command will add user to the specific group

### File Operations:

- `touch file1` - Create file1
- `cat file1 file2` - Concatinate file and provide ouput.
- `less file1` - View and paginate file1
-  `file file1` - Get type of file1
- `cp file1 file2` - Copy file1 to file2
- `mv file1 file2` - Move file1 to file2
- `rm file1` - Delete file1

### Directory Operations:

- `pwd` - Show current directory
- `mkdir dir` - Make directory dir
- `cd dir` - Change directory to dir
- `cd ..` - Fo up a directory
- `ls` - List files

### ls operations:

- `-a` - Show all files
- `-R` - Recursive list
- `-r` - Reverse Order
- `-t` - Sort by last modified
- `-S` - Sort by file size
- `-l` - Long listing format
- `-1` - One file per line
- `-m` - Comma-seperated output
- `-Q` - Quoted output

