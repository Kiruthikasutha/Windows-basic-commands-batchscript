# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript

# AIM:
To execute Windows basic commands and batch scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Windows environment installed on the system or installed inside a virtual environment like virtual box/vmware 

### Step 2:

Write the Windows commands / batch file
Save each script in a file with a .bat extension.
Ensure you have the necessary permissions to perform the operations.
Adapt paths as needed based on your system configuration.
### Step 3:

Execute the necessary commands/batch file for the desired output. 




# WINDOWS COMMANDS:
## Exercise 1: Basic Directory and File Operations
Create a directory named "MyLab" on the desktop.
```
mkdir %userprofile%\Desktop\MyLab
```
![Screenshot 2024-05-17 184059](https://github.com/Kiruthikasutha/Windows-basic-commands-batchscript/assets/144979570/9b9ed49a-9a24-4956-83f0-5139786c6323)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.



## COMMAND AND OUTPUT

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.
```
cd %userprofile%\Desktop\MyLab
```
![Screenshot 2024-05-17 184114](https://github.com/Kiruthikasutha/Windows-basic-commands-batchscript/assets/144979570/977bc75f-cc6a-4a07-81cf-b669dc91e895)
![Screenshot 2024-05-17 184123](https://github.com/Kiruthikasutha/Windows-basic-commands-batchscript/assets/144979570/9b1ab827-077e-4b63-b82b-d8439967c5ab)



## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
```
dir %userprofile%\Desktop\MyLab
```
![Screenshot 2024-05-17 184133](https://github.com/Kiruthikasutha/Windows-basic-commands-batchscript/assets/144979570/03936097-34e2-4e9e-aea3-4d2c8eab603b)


## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.
```
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup
```
![Screenshot 2024-05-17 184144](https://github.com/Kiruthikasutha/Windows-basic-commands-batchscript/assets/144979570/a6eae73a-640b-4a7c-a750-dcb81f40b565)
![Screenshot 2024-05-17 184150](https://github.com/Kiruthikasutha/Windows-basic-commands-batchscript/assets/144979570/57df020f-c179-4a2e-9b41-077f379cec38)



## COMMAND AND OUTPUT
```
mv Myfile.txt %userprofile%\Documents
```
![Screenshot 2024-05-17 184159](https://github.com/Kiruthikasutha/Windows-basic-commands-batchscript/assets/144979570/f3eb580c-2c8a-4842-b328-64b873f7b8b9)



## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```
Modify the script to delete files with the ".docx" extension from the "Documents" folder after creating the backup.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```

## OUTPUT

![Screenshot 2024-05-17 184221](https://github.com/Kiruthikasutha/Windows-basic-commands-batchscript/assets/144979570/5fa60a46-242d-4237-a818-5839b230be7c)

# RESULT:
The commands/batch files are executed successfully.

