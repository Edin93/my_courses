# The shell (sh):
- it's a CLI (command line interface).
- it's a program that takes commands from the keyboard and gives them to the OS to perform.
- on most unix-like systems, there's a program called bash that acts as the shell program. there are other shell programs.

# Terminal:
- a program called terminal emulator.
- it opens a window and lets you interact with the shell.

#Navigation:

## pwd
- print working directory

## cd
- change directory.
- change directory with a relative path or an absolute path:
*a relative path is relative to your current working directory.
*an absolute path is from the root (starts with /).
- cd shortcuts:
*cd ---> changes the working directory to your home.
*cd / ---> changes the working directory to the root.
* cd - ---> changes the working directory to the previous one.
* cd ~user_name ---> changes the working directory to the home directory of the specified user.

## ls
- list files and subdirectories.

## file
- will examine the file and tell you what kind of file it is (what kind of data the file contains).
- symbolic link are a special type of file that points to another file.

# Files manipulation:
- cp: copy files and directories.
- mv: move or rename files and directories.
- rm: remove files and directories.
- mkdir: craete directories.

# Working with commands:
- type: display information about command type.
- which: locate the command.
- help: display reference page for shell builtin.
- man: display on-line command reference.

# 4 Types of commands:
- Executable program.
- a command built into the shell itself: bash provides a number of commands called shell builtins, ex: cd.
- Shell function: miniature shell scripts incorporated into the environment.
- Alias: commands that you can define yourselves, built from other commands.

# Shebang:
- #! that's a shebang.
- added at the start of scripts.
- in unix-like OS, when a text file starts with shebang, it's used as if an executable program.

# Permissions:
- file permissions: owner permissions- group permissions - others permissions.
- chmod: modify files and directories access rights.
- su: temporarily become the superuser.
- sudo: temporarily become the superuser.
- chown: change file ownership.(ex chown new_user file).
- chgrp: change file group's ownership. (ex chgrp chgrp new_group file). you must be the owner of the file or directory to perform chgrp.
- id: print user and group information for the specified user, if no user specified, then for current user.
- whoami: print the username of the current effective user ID.
- adduser, addgroup: add a user or group to the system.
- useradd: create new user or update new user information.

# base2 (binary) ---> base8 (octal)
- rwx: 111 ---> 7
- rw-: 110 ---> 6
- r-x: 101 ---> 5
- -x: 101 ---> 5
- r--: 100 ---> 4
- ---: 000 ---> 0

# RWX meaning for files permissions:
- RWX: means read, write and execute permissions for files.

# RWX meaning for directories permissions:
- r: to list the directory content, if x is set.
- w: to create, delete or rename files, in the directory, if x is set also.
- x: to enter the directory (cd directory).

# Others
-wc: prints the number of: Lines Words Characters.
# RESOURCES
- [Useful bash shortcuts](https://www.howtogeek.com/howto/ubuntu/keyboard-shortcuts-for-bash-command-shell-for-ubuntu-debian-suse-redhat-linux-etc/)
