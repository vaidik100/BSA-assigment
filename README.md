# BSA-assigment

• Author details:
  Vaidik Kakadiya
  1000114909
  23/05/2024
  
• Project details for each of the two scripts:
8IN616 – Operating Systems Concepts
Bash Scripting Assignment
–Task1:
The purpose of the script is to automate the user creation process on a Linux system based on information provided in a CSV file. Here's a summary of the script's purpose:

Automated User Creation: The script reads user information from a CSV file, including email, birth date, groups, and shared folder. It then creates user accounts based on this information.

Password Generation: It generates default passwords for the user accounts using the birth dates provided in the CSV file. If the generated password is less than 8 characters, it appends additional characters to meet the minimum length requirement.

Group Management: It creates groups and adds users to specified groups based on the information provided in the CSV file. If a group does not exist, it creates the group before adding the user to it.

Shared Folder Setup: If a shared folder is specified in the CSV file for a user, the script creates the shared folder, sets appropriate permissions, and creates a symbolic link to the shared folder in the user's home directory.

Sudo Alias Creation: For users who are members of the sudo group (users with administrative privileges), the script creates an alias (myls) in their .bash_aliases file to display hidden files and permissions in their home directory.

Logging: The script logs informational messages and errors to a log file (script.log) for monitoring and troubleshooting purposes.

Overall, the script streamlines the process of user management on a Linux system by automating user creation, group management, shared folder setup, and providing administrative users with helpful aliases.

Task2:

Directory Existence Check: The script checks if the specified directory exists. If the directory doesn't exist, it logs an error message and exits.

Directory Compression: It compresses the specified directory into a .tar.gz archive using the tar command.

Remote Server Details: The script prompts the user to enter the IP address or URL of the remote server, the port number, and the target directory on the remote server where the compressed file will be uploaded.

File Upload: It uploads the compressed file to the remote server using SCP. Any errors that occur during the upload process are logged.

Local Archive Cleanup: After successful upload, the local compressed archive is removed to save disk space.

Logging: All actions performed by the script, including errors and informational messages, are logged to a specified log file (backup.log).

Overall, the script provides a convenient way to back up directories by compressing them and uploading the compressed files to a remote server, while also ensuring error handling and logging for robustness and monitoring purposes.

To run the Task 1:
Enter the the specific directory of PC: 
chmod +x /directory/vaidik.sh

sudo /directory/vaidik.sh /directory/users.csv

To run the Task 2:
Enter the the specific directory of PC: 
chmod +x /directory/backup.sh

sudo /directory/backup.sh 
