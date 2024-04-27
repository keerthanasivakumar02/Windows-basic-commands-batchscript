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
```
mkdir %userprofile%\Desktop\MyLab
```
![image](https://github.com/keerthanasivakumar02/Windows-basic-commands-batchscript/assets/150827397/d8bb33e5-863c-4e6e-9443-bf0a64234331)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
```
cd %userprofile%\Desktop\MyLab
```
![image](https://github.com/keerthanasivakumar02/Windows-basic-commands-batchscript/assets/150827397/b381c59c-0237-446f-a6f2-309e741ddfa2)
![image](https://github.com/keerthanasivakumar02/Windows-basic-commands-batchscript/assets/150827397/2b45b308-a9ca-4ddd-b073-4aea0c8e7a16)

List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
```
dir %userprofile%\Desktop\MyLab
```
![image](https://github.com/keerthanasivakumar02/Windows-basic-commands-batchscript/assets/150827397/9dddd277-5c77-470a-9398-d46d3f999077)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup
```
![image](https://github.com/keerthanasivakumar02/Windows-basic-commands-batchscript/assets/150827397/ba586a1b-fbb5-45b4-ad6f-4718a7ee9e29)
![image](https://github.com/keerthanasivakumar02/Windows-basic-commands-batchscript/assets/150827397/425d8f84-fd98-4f5c-895f-9bd7244074d3)

Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
```
mv Myfile.txt %userprofile%\Documents
```
![image](https://github.com/keerthanasivakumar02/Windows-basic-commands-batchscript/assets/150827397/d274f8c9-420d-43a6-96ef-b471592d3715)

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


![image](https://github.com/keerthanasivakumar02/Windows-basic-commands-batchscript/assets/150827397/a3a97c18-4cd3-40d7-817a-a78f5f2bd644)



# RESULT:
The commands/batch files are executed successfully.

