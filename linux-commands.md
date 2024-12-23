Here’s a well-structured guide for essential Linux commands:

# Linux Command Reference Guide

A practical guide to commonly used Linux commands for system management, file operations, and troubleshooting.

---

## Basic Commands
1. **`pwd`**: Prints the current working directory.
2. **`ls`**: Lists files and directories in the current directory.
   - **`ls -l`**: Lists files with detailed information (permissions, owner, size, etc.).
   - **`ls -a`**: Includes hidden files in the listing.
3. **`cd <directory>`**: Changes the current directory to the specified one.
4. **`mkdir <directory_name>`**: Creates a new directory.
5. **`rmdir <directory_name>`**: Removes an empty directory.

---

## File Management
6. **`touch <file_name>`**: Creates an empty file or updates the timestamp of an existing file.
7. **`cat <file_name>`**: Displays the content of a file.
8. **`cp <source> <destination>`**: Copies a file or directory.
   - Use **`cp -r`** for recursive copying of directories.
9. **`mv <source> <destination>`**: Moves or renames a file or directory.
10. **`rm <file_name>`**: Deletes a file.
    - Use **`rm -r <directory>`** to delete a directory and its contents.

---

## File Permissions and Ownership
11. **`chmod <permissions> <file_name>`**: Changes the permissions of a file or directory.
    - Example: **`chmod 755 <file>`** sets read, write, execute for the owner and read, execute for others.
12. **`chown <user>:<group> <file_name>`**: Changes the ownership of a file or directory.

---

## Process Management
13. **`ps`**: Lists running processes.
    - **`ps aux`**: Shows detailed information about all processes.
14. **`top`**: Displays a real-time view of system processes and resource usage.
15. **`kill <PID>`**: Sends a signal (default: terminate) to a process.
16. **`kill -9 <PID>`**: Forcefully terminates a process.
17. **`jobs`**: Lists background jobs in the current shell.
18. **`fg <job_number>`**: Brings a background job to the foreground.

---

## User Management
19. **`whoami`**: Displays the current logged-in user.
20. **`who`**: Shows information about all logged-in users.
21. **`adduser <username>`**: Creates a new user.
22. **`passwd <username>`**: Changes the password for a user.
23. **`su <username>`**: Switches to another user account.
24. **`sudo <command>`**: Executes a command with root privileges.

---

## Networking
25. **`ping <host>`**: Checks connectivity to a host.
26. **`ifconfig`**: Displays network interface configurations.
27. **`ip addr`**: Shows IP addresses and interface details.
28. **`netstat`**: Lists network connections, routing tables, and interface statistics.
29. **`curl <url>`**: Fetches data from a URL.
30. **`wget <url>`**: Downloads files from a URL.

---

## Disk and File System Management
31. **`df -h`**: Displays disk usage of mounted file systems in a human-readable format.
32. **`du -sh <directory>`**: Shows the total size of a directory.
33. **`mount <device> <mount_point>`**: Mounts a device to a directory.
34. **`umount <device>`**: Unmounts a device.
35. **`lsblk`**: Lists information about block devices.
36. **`fdisk -l`**: Displays information about disk partitions.

---

## Archiving and Compression
37. **`tar -cvf <archive_name.tar> <file_or_directory>`**: Creates a tar archive.
38. **`tar -xvf <archive_name.tar>`**: Extracts a tar archive.
39. **`gzip <file>`**: Compresses a file using gzip.
40. **`gunzip <file.gz>`**: Decompresses a gzip file.

---

## Searching and Filtering
41. **`grep <pattern> <file>`**: Searches for a pattern in a file.
42. **`find <directory> -name <file_name>`**: Searches for a file in a directory.
43. **`locate <file_name>`**: Quickly finds a file using a pre-built index.
44. **`head -n <number> <file>`**: Displays the first few lines of a file.
45. **`tail -n <number> <file>`**: Displays the last few lines of a file.

---

## System Monitoring
46. **`uptime`**: Displays system uptime and load averages.
47. **`free -h`**: Shows memory usage in a human-readable format.
48. **`dmesg`**: Displays system kernel messages.
49. **`iostat`**: Provides CPU and I/O statistics.
50. **`vmstat`**: Displays system performance statistics.

---

## Package Management (Debian-based)
51. **`apt-get update`**: Updates the package lists for available upgrades.
52. **`apt-get upgrade`**: Installs available package updates.
53. **`apt-get install <package>`**: Installs a specified package.
54. **`apt-get remove <package>`**: Removes a specified package.

---

## Debugging and Troubleshooting
55. **`strace <command>`**: Traces system calls made by a command.
56. **`lsof`**: Lists open files and their processes.
57. **`systemctl status <service>`**: Checks the status of a systemd service.
58. **`journalctl -u <service>`**: Views logs for a specific service.
59. **`history`**: Displays the command history for the current session.

---


## Variables and Environment
60. **`echo $VARIABLE_NAME`**: Displays the value of an environment variable.
61. **`export VARIABLE_NAME=value`**: Sets an environment variable for the current session.
62. **`unset VARIABLE_NAME`**: Removes an environment variable.

---

## Loops and Conditionals
63. **`if [ condition ]; then ... fi`**: Executes commands based on a condition.
64. **`for var in list; do ... done`**: Iterates over a list of items.
65. **`while [ condition ]; do ... done`**: Loops while a condition is true.
66. **`break`**: Exits a loop prematurely.
67. **`continue`**: Skips the current loop iteration.

---

## Functions and Scripts
68. **Defining a function**:
    ```bash
    my_function() {
        echo "Hello, Bash!"
    }
    ```
69. **Running a script**:
    ```bash
    ./script_name.sh
    ```
    - Make it executable with **`chmod +x script_name.sh`**.
70. **Passing arguments to a script**:
    - `$1, $2, ...`: Access command-line arguments in a script.
    - **Example**:
        ```bash
        echo "First argument: $1"
        ```

---

This guide provides a quick reference for common Linux commands to help you efficiently manage files, processes, users, and system resources. Bookmark it for easy access!
