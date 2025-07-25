# File-Permission-Modification-in-Ubuntu
This terminal session demonstrates the process of modifying file permissions in an Ubuntu environment running on Oracle VirtualBox. The user performed the following actions:
Initial Directory Listing:

Used ls -la to display all files with detailed permissions in the Music directory

Showed three items:

Two directories (wpj.asp) with different permissions

One Python file (main.py) with initial permissions -rw-rw-r-- (664)

Permission Modification:

Executed sudo chmod 775 main.py to change permissions

Entered the sudo password when prompted

The octal value 775 corresponds to -rwxrwxr-x permissions

Verification:

Ran ls -la again to confirm the permission change

The new permissions for main.py were successfully set to -rwxrwxr-x

Permission Breakdown
Original Permissions (-rw-rw-r--)
User: Read + Write (rw-)

Group: Read + Write (rw-)

Other: Read only (r--)

New Permissions (-rwxrwxr-x) after chmod 775
User: Read + Write + Execute (rwx)

Group: Read + Write + Execute (rwx)

Other: Read + Execute (r-x)

Key Observations
The sudo command was required to modify the file permissions

The octal mode 775 successfully granted execute permissions to all users while maintaining different access levels

The directory permissions remained unchanged during this operation

The file size (7 bytes) suggests main.py is a very small Python script

This session demonstrates a common workflow for adjusting file permissions in Linux systems, particularly when needing to make scripts executable.

