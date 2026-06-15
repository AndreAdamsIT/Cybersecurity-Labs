# Basic Linux Commands

## pwd
Purpose: Shows the current working directory.

Example:
pwd

## ls
Purpose: Lists files and directories.

Example:
ls

## cd
Purpose: Changes directories.

Example:
cd Documents

## mkdir
Purpose: Creates a new directory.

Example:
mkdir Projects

## cat
Purpose: Displays the contents of a file.

Example:
cat notes.txt

## echo
Purpose: Displays text in the terminal.

Example:

echo "Hello World!"

## Comments
Linux ignores anything after the # symbol on a line.

Purpose: Add notes and explanations that Linux ignores.

Syntax:

# This is a comment

Example:

# Print a welcome message
echo "Hello World!"

## touch
Purpose: Creates a new empty file.

Example:
touch hello.txt

Notes:
- Creates an empty file.
- Can create multiple files at once:
  touch file1.txt file2.txt file3.txt
- If the file already exists, it updates the timestamp instead of overwriting the file.

## grep

Purpose: Searches the contents of files for specific text or patterns.

Example:
grep "THM" access.log

Explanation:
Searches the file `access.log` and displays every line containing the text `THM`.

Example:
grep -R "PRETTY_NAME" /etc/

Explanation:
Searches recursively through all files and subdirectories inside `/etc/` for the text `PRETTY_NAME`.

Notes:
- Searches inside files, not filenames.
- `-R` searches recursively through subdirectories.
- `-i` performs a case-insensitive search.
- Useful for finding errors, usernames, IP addresses, configuration settings, or log entries.

Real-World Use:
IT Support and Cybersecurity professionals use `grep` to search log files, configuration files, and system outputs for errors, IP addresses, usernames, failed logins, and other important information.

Examples:
grep "error" system.log
grep "admin" users.txt
grep -i "failed" auth.log
grep -R "password" /etc/
