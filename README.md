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


## COMMAND AND OUTPUT

mkdir %userprofile%\Desktop\MyLab

![8th 1](https://github.com/Alfredsec/Windows-basic-commands-batchscript/assets/120621608/f8f0e292-bcb4-4d3d-9267-bec535e665a4)


Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT


cd %userprofile%\Desktop\MyLab

![8th 2](https://github.com/Alfredsec/Windows-basic-commands-batchscript/assets/120621608/f00304e8-7e06-47ef-b6c7-271932f85bc4)

![8th 3](https://github.com/Alfredsec/Windows-basic-commands-batchscript/assets/120621608/5dde6b60-9c92-472e-9927-fc93980b397e)


List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT

dir %userprofile%\Desktop\MyLab

![8th 4](https://github.com/Alfredsec/Windows-basic-commands-batchscript/assets/120621608/b1aad3d0-448a-4faf-8f12-bc6c4c02cd92)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT

mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup

![8th 5](https://github.com/Alfredsec/Windows-basic-commands-batchscript/assets/120621608/66226eef-04b2-4982-966f-8677019c7f04)

![8th 6](https://github.com/Alfredsec/Windows-basic-commands-batchscript/assets/120621608/fc100610-cda2-46dd-971a-004c571ddcb7)

Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT

mv Myfile.txt %userprofile%\Documents

![8th 7](https://github.com/Alfredsec/Windows-basic-commands-batchscript/assets/120621608/9472a64c-5716-4a95-a7cc-92d7a479b38f)


## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```
Modify the script to delete files with the ".docx" extension from the "Documents" folder after creating the backup
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```


## OUTPUT

![8th 8](https://github.com/Alfredsec/Windows-basic-commands-batchscript/assets/120621608/9263c5b3-369a-461a-aa6f-39c36201484d)


# RESULT:
The commands/batch files are executed successfully.

