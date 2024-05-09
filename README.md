# Windows-basic-commands-batchscript
# Ex08-Windows-basic-commands-batchscript

## Developed by: DURGADEVI P
## Register Number: 212223100006

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

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.
mkdir %userprofile%\Desktop\MyLab

![image](https://github.com/durgadevi22d/Windows-basic-commands-batchscript/assets/149987216/c126114c-ebe7-4b3e-b9fa-321fd850a91e)


## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.
cd %userprofile%\Desktop\MyLab

![image](https://github.com/durgadevi22d/Windows-basic-commands-batchscript/assets/149987216/a76bbdc8-f4e0-47ea-9711-49fa7e22e9f1)
![image](https://github.com/durgadevi22d/Windows-basic-commands-batchscript/assets/149987216/082ff9b8-5d8f-4dc4-a2e7-0c63273ae0e0)


## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
dir %userprofile%\Desktop\MyLab

![image](https://github.com/durgadevi22d/Windows-basic-commands-batchscript/assets/149987216/2eabdd8c-51b2-4f5a-a550-f35bf2b73c56)


## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup

![image](https://github.com/durgadevi22d/Windows-basic-commands-batchscript/assets/149987216/0101d370-8ee2-4072-ab24-9288edba641b)
![image](https://github.com/durgadevi22d/Windows-basic-commands-batchscript/assets/149987216/a9c13c7d-d5d3-416d-ae86-f5d5b1f9fa87)



## COMMAND AND OUTPUT

mv Myfile.txt %userprofile%\Documents


![image](https://github.com/durgadevi22d/Windows-basic-commands-batchscript/assets/149987216/7e954417-c8d1-4585-9060-bf19a0cd5a42)



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

![image](https://github.com/durgadevi22d/Windows-basic-commands-batchscript/assets/149987216/6e976458-f53a-4464-9c87-1535335d5435)

# RESULT:
The commands/batch files are executed successfully.

