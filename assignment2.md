
QUESTION: Describe the purpose of the following Linux commands. Your descriptions should be concise yet comprehensive.

ANSWER: 
ls: Lists the files and directories in a directory. It is a fundamental command for navigating the file system.

ln: Creates links between files. The most common use is to create a symbolic link (or "symlink"), which acts as a shortcut to another file or directory.

type: Describes how a command name is interpreted. It can tell you if a command is an alias, a built-in shell command, or an executable file located in the system's PATH.

which: Locates the executable file associated with a given command. It searches the system's PATH to find the full path of the command that will be executed.

man: Displays the manual page (short for "manual") for a command. This provides a detailed reference, including a command's syntax, options, and examples.

head: Outputs the first 10 lines of a file by default. It is useful for quickly previewing the beginning of a file without having to open the entire thing.

tail: Outputs the last 10 lines of a file by default. It is frequently used with the -f (follow) option to monitor a log file in real-time as new information is appended.

less: A powerful program for viewing the contents of a file one screen at a time. It is much more efficient than cat for large files as it allows for forward and backward scrolling.


QUESTION: Explain the function of each command listed below. For each one, provide a practical example of its use, along with a brief explanation of what the example command accomplishes.

ANSWER: 
curl: A command-line tool for transferring data to or from a server. It supports various protocols like HTTP, FTP, and more.

Example: curl https://www.example.com

Explanation: This command retrieves the HTML content from the specified website and prints it to the terminal.

cat: Short for "concatenate," this command reads file contents and prints them to the standard output. It can also be used to combine the contents of multiple files.

Example: cat document.txt

Explanation: This command displays the entire content of the file document.txt in the terminal.

chmod: Used to change the access permissions of files and directories. Permissions are set for the owner, group, and others and control whether they can read, write, or execute the file.

Example: chmod 755 script.sh

Explanation: This command sets the permissions for script.sh. The owner has read, write, and execute permissions (7), while the group and others have read and execute permissions (5).

su: Used to switch to another user account. By default, it attempts to switch to the root user.

Example: su -

Explanation: This command switches the current user to the root user, prompting for the root user's password. The hyphen (-) ensures that the environment is fully loaded for the new user.

sudo: Allows a permitted user to execute a command as another user (most commonly the root user). It requires the current user's password.

Example: sudo apt update

Explanation: This command executes the apt update command with administrative privileges, allowing the system's package list to be updated.

grep: A powerful tool for searching for a pattern within text files. It searches for a regular expression and prints any lines that match.

Example: grep "error" /var/log/syslog

Explanation: This command searches for and displays all lines containing the word "error" in the /var/log/syslog file.

QUESTION: Discuss the difference between the ps and top commands. Explain the primary use case for each one and why they are both valuable tools for monitoring a system.

ANSWER: 
Both ps and top are used to view and monitor running processes on a Linux system, but they differ significantly in their functionality and output.

The ps command provides a static snapshot of the processes. When you run ps, it captures the state of the processes at that precise moment and displays the information. This makes it ideal for use in shell scripts or when you need to quickly check the status of a specific process without needing a real-time view. Its primary use is often to find a specific process ID (PID) to then perform an action like killing the process.

In contrast, the top command provides a real-time, dynamic view of the system's processes. It is an interactive tool that continuously updates the display, showing a live list of processes sorted by resource usage (CPU, memory, etc.). The primary use case for top is for real-time performance monitoring and troubleshooting. It allows a user to immediately see which processes are consuming the most resources and to react accordingly.

In summary, ps is for a one-time view of processes at a single moment, whereas top is for continuous monitoring of system performance. Both are essential for system administration and debugging.
