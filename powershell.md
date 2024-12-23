Here’s your README.md file for Windows PowerShell:

# Windows PowerShell Command Reference Guide

A comprehensive guide to commonly used PowerShell commands, operations, and features for scripting, file management, and system administration.

---

## Getting Started
1. **`$PSVersionTable.PSVersion`**: Displays the installed PowerShell version.
2. **`Get-Command`**: Lists all available PowerShell commands.
3. **`Start-Process powershell`**: Launches a new PowerShell session.
4. **`exit`**: Exits the current PowerShell session.

---

## File and Directory Operations
5. **`Get-Location`**: Prints the current working directory.
6. **`Get-ChildItem`**: Lists files and directories in the current directory.
   - **`Get-ChildItem -Recurse`**: Lists all files and directories recursively.
7. **`Set-Location <directory>`**: Changes the current directory.
8. **`New-Item -ItemType Directory -Name <directory_name>`**: Creates a new directory.
9. **`Remove-Item <item>`**: Deletes a file or directory.
    - **`Remove-Item -Recurse <directory>`**: Deletes a directory and its contents recursively.
10. **`Copy-Item <source> <destination>`**: Copies a file or directory.
11. **`Move-Item <source> <destination>`**: Moves or renames files or directories.

---

## File Viewing and Editing
12. **`Get-Content <file>`**: Displays the content of a file.
13. **`Set-Content <file> -Value <text>`**: Writes text to a file, overwriting the existing content.
14. **`Add-Content <file> -Value <text>`**: Appends text to a file.
15. **`Out-File <file>`**: Redirects command output to a file.
16. **`Notepad <file>`**: Opens a file in Notepad for editing.

---

## Process Management
17. **`Get-Process`**: Displays running processes.
18. **`Stop-Process -Id <PID>`**: Terminates a process by its Process ID (PID).
19. **`Start-Job -ScriptBlock { <command> }`**: Starts a background job.
20. **`Get-Job`**: Lists all background jobs.
21. **`Receive-Job -Id <job_id>`**: Retrieves the output of a background job.
22. **`Stop-Job -Id <job_id>`**: Stops a background job.

---

## Variables and Environment
23. **`$Env:<variable_name>`**: Displays the value of an environment variable.
24. **`$VariableName = <value>`**: Sets a variable in the current session.
25. **`Remove-Variable <variable_name>`**: Removes a variable.
26. **`Set-EnvironmentVariable -Name <name> -Value <value>`**: Sets a permanent environment variable.

---

## Loops and Conditionals
27. **`if (<condition>) { ... } else { ... }`**: Executes commands based on a condition.
28. **`foreach ($item in <collection>) { ... }`**: Iterates over a collection of items.
29. **`while (<condition>) { ... }`**: Loops while a condition is true.
30. **`break`**: Exits a loop prematurely.
31. **`continue`**: Skips the current iteration of a loop.

---

## Functions and Scripts
32. **Defining a function**:
    ```powershell
    function My-Function {
        Write-Output "Hello, PowerShell!"
    }
    ```
33. **Running a script**:
    ```powershell
    .\script_name.ps1
    ```
    - Allow script execution with **`Set-ExecutionPolicy RemoteSigned`**.
34. **Passing arguments to a script**:
    - `$args[0], $args[1], ...`: Access command-line arguments in a script.
    - **Example**:
        ```powershell
        Write-Output "First argument: $($args[0])"
        ```

---

## File Permissions
35. **`Get-Acl <file>`**: Displays the permissions of a file or directory.
36. **`Set-Acl <file> -AclObject <acl>`**: Changes file permissions.
37. **`icacls <file>`**: Modifies file and folder permissions from the command line.

---

## Networking
38. **`Test-Connection <host>`**: Tests connectivity to a host (similar to `ping`).
39. **`Invoke-WebRequest <url>`**: Fetches data from a URL.
40. **`Start-BitsTransfer -Source <url> -Destination <path>`**: Downloads files from a URL.
41. **`Get-NetIPAddress`**: Displays network adapter IP addresses.

---

## Debugging
42. **`Set-PSDebug -Trace 1`**: Enables script debugging.
43. **`Set-PSDebug -Off`**: Disables debugging.
44. **`Get-Error`**: Displays the last error that occurred.
45. **`Trap { <command> }`**: Executes a command when an error is encountered.

---

## Searching and Filtering
46. **`Select-String -Pattern <text> -Path <file>`**: Searches for a pattern in a file.
47. **`Get-ChildItem -Filter <pattern>`**: Filters files and directories by pattern.
48. **`Where-Object { <condition> }`**: Filters objects based on a condition.
49. **`ForEach-Object { <command> }`**: Processes each item in a collection.
50. **`Out-GridView`**: Displays output in an interactive grid.

---

## System Information
51. **`Get-ComputerInfo`**: Displays system information.
52. **`Get-PSDrive`**: Lists available drives.
53. **`Get-Disk`**: Displays information about connected disks.
54. **`Get-Uptime`**: Shows system uptime.
55. **`Get-Process | Measure-Object -Property CPU -Sum`**: Displays total CPU usage.

---

## Archiving and Compression
56. **`Compress-Archive -Path <file_or_directory> -DestinationPath <archive.zip>`**: Creates a zip archive.
57. **`Expand-Archive -Path <archive.zip> -DestinationPath <directory>`**: Extracts a zip archive.
58. **`Copy-Item <source> -Destination <destination> -Compress`**: Compresses files during copy.

---

This guide covers essential PowerShell commands and concepts to help you efficiently manage your system and write scripts. Bookmark it for quick reference!
