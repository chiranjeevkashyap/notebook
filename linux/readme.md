# Linux 

## Table of Content
- [Linux](#linux-crash-course)
    - [Day 1 – Linux File System](#day-1--linux-file-system)
- [Commands](#linux-commands)
    - [Basic Command](#basic)

## Linux Crash Course

### Day 1 – Linux File System

Learn the Directory Structure

```linux
ls /
```

| Directory | Purpose                     |
| --------- | --------------------------- |
| `/`       | Root of the filesystem      |
| `/home`   | User home directories       |
| `/root`   | Root user's home            |
| `/etc`    | Configuration files         |
| `/var`    | Logs, caches, variable data |
| `/usr`    | Installed applications      |
| `/bin`    | Essential commands          |
| `/lib`    | Libraries                   |
| `/tmp`    | Temporary files             |
| `/opt`    | Optional software           |
| `/srv`    | Data served by services     |
| `/mnt`    | Temporary mount points      |
| `/media`  | Removable media             |
| `/dev`    | Devices                     |
| `/proc`   | Process information         |
| `/sys`    | Kernel information          |

- `rm -r folder_name`: Deletes a non-empty directory and all its files/subfolders.
- `rm -rf folder_name`: Forces the deletion permanently without asking for confirmation.
- `rmdir folder_name`: Deletes a directory only if it is completely empty.


## [Engineering Digest Linux Course (Vipul Tyagi)](https://youtube.com/playlist?list=PLA3GkZPtsafbK3YyxdRzF5yh1TuwGn_Lu&si=7NVPoNapH9vZNOML)

## Basic Linux Command are divided into 3 parts
 `Command Name` + `Options` (optional & needed) + `Arguments`

1. `cat`: its used to read content in a file
    - example: `cat example.txt`
    - options
        - `-n`: its used to print line numbers.
        - `--number`: working is same its just full name of command.

2. `ALT+L` or `clear`: its used to clear the terminal

3. `ls`: its used to see file or folder inside working directory.

4. `ncal`: its used to see current month calendar.
    - firstly, you should have to installed the ncal in your system, ubuntu command: `sudo apt ncal`
    - options
        - `ncal 2022`: complete calendar of 2022
        - `ncal july 2022`: 2022 july calendar
        - `ncal may 2022 -w`: 2022 may calendar with week number
        - `ncal may 2022 -w -M`: 2022 may calendar with week number and start week from monday.
        - `ncal may 2022 -wM`: just shorthand command


## Linux Commands

### Basic

| action | command | description |
| --- | --- | --- |
| Standard Rename | mv old_name new _name | Its used to rename the directory. |
| Standard folder | rm -r folder_name| This removes the directory and all its contents recursively.|
| Safe/Interactive delete | rm -ri folder_name | This will prompt you for confirmation before deleting each item, helping prevent accidents. |
| Force delete (High Risk) | rm -rf folder_name | This forces the removal of everything in the folder without any confirmation prompts. Use extreme caution, especially with wildcards or absolute paths, as this can delete critical data instantly. |
| Folders requiring root permissions | sudo rm -rf folder_name | This uses administrative privileges to delete folders protected by the system. Only use sudo for files you are certain are safe to remove.|
| Empty folders only | rmdir folder_name | This is the safest command as it only works if the folder is completely empty.|
| List of all installed tools | apt list --installed | To see which tools and programs are installed on your Ubuntu system |
| List of all installed tools by user | apt-mark showmanual | to see only the tools and programs you installed yourself (hiding automatic dependencies). |