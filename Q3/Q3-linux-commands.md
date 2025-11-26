Q3 – Linux Based User Management  
Amazon Linux Machine  
Project: “Hdfc_Bank-ClientApp”

In this task, we were asked to perform basic Linux user management operations for a company setup where:
- Team A (Developers): Developer1, Developer2, Developer3
- Team B (Testers): Tester1, Tester2
- A new developer “Developer4” has joined
- Developer3 has left the company
- A project zip file “Hdfc-Pack” needs to be inspected and modified

Below are the operations I performed along with the commands and explanations.

------------------------------------------------------------
1. Adding a New User “Developer4” to Developer Group
------------------------------------------------------------

Command used:
sudo useradd -m -G Developer Developer4
sudo passwd Developer4
id Developer4

Explanation (in simple words):
- “useradd” creates a new user named Developer4.
- The “-m” option creates a home directory for the user automatically.
- “-G Developer” means the user is added to the Developer group.
- “passwd” is used to set a password for the new user.
- “id Developer4” helps me confirm that the user has been created successfully and is actually part of the Developer group.

Outcome:
Developer4 is added and properly assigned to the Developer team.

------------------------------------------------------------
2. Removing “Developer3” Completely (User + Home Directory)
------------------------------------------------------------

Command used:
sudo userdel -r Developer3
id Developer3
ls /home/

Explanation:
- “userdel -r” deletes the user AND also removes their home folder.
- Running “id Developer3” after deletion should give an error like “no such user,” which confirms removal.
- “ls /home/” is used just to double-check that Developer3’s home directory is gone.

Outcome:
Developer3’s account and all files were removed from the system.

------------------------------------------------------------
3. Checking Contents of “Hdfc-Pack.zip” and Removing a File
------------------------------------------------------------

Step A: View what’s inside the zip file
Command:
unzip -l Hdfc-Pack.zip

What it does:
This command lists all the files inside the zip without extracting anything. It helps me see which files exist before deleting anything.

Step B: Delete a specific file from inside the zip
Command:
zip -d Hdfc-Pack.zip <file_to_remove>

For example:
zip -d Hdfc-Pack.zip config/app.properties

Explanation:
- “zip -d” allows us to delete a file from a ZIP archive directly.
- It removes only the selected file and keeps the rest intact.

Step C: Confirm deletion
Command:
unzip -l Hdfc-Pack.zip

This lets me verify that the file I deleted no longer appears inside the ZIP.

Outcome:
The ZIP file was inspected, and the required file inside it was successfully removed.

Summary:
- I added the new user Developer4 and placed them into the Developer group.
- I removed Developer3 completely, including their home folder.
- I opened the Hdfc-Pack zip file, checked all its contents, and deleted one file from it without extracting the entire archive.

End of Q3 Report.
