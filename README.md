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

![Screenshot 2024-04-27 180635](https://github.com/RahulKrishna05/Windows-basic-commands-batchscript/assets/162027231/53b98506-0f18-4d72-aa52-32dcfdc509a1)




Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
cd %userprofile%\Desktop\MyLab

![Screenshot 2024-04-27 180650](https://github.com/RahulKrishna05/Windows-basic-commands-batchscript/assets/162027231/725fa54e-d8b8-4969-805e-bf5b17ea042b)
![Screenshot 2024-04-27 180705](https://github.com/RahulKrishna05/Windows-basic-commands-batchscript/assets/162027231/bf24ae91-2ec6-40ff-aa81-e0ef7c19dbd5)


List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
dir %userprofile%\Desktop\MyLab

![Screenshot 2024-04-27 180716](https://github.com/RahulKrishna05/Windows-basic-commands-batchscript/assets/162027231/668e265e-8830-4342-86b1-549bd4fda87d)


Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT

mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup


![Screenshot 2024-04-27 180726](https://github.com/RahulKrishna05/Windows-basic-commands-batchscript/assets/162027231/5d1c71f7-c141-49f0-821c-ec67ab8a721f)

![Screenshot 2024-04-27 180735](https://github.com/RahulKrishna05/Windows-basic-commands-batchscript/assets/162027231/3fc34cfa-c013-414e-a0b7-7a30282f3cc9)


Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
mv Myfile.txt %userprofile%\Documents


![Screenshot 2024-04-27 180756](https://github.com/RahulKrishna05/Windows-basic-commands-batchscript/assets/162027231/ccf37aee-776d-4647-b6b1-3543ae6faf1f)



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



![Screenshot 2024-04-27 180807](https://github.com/RahulKrishna05/Windows-basic-commands-batchscript/assets/162027231/a9708aaa-0cb4-40c8-9ea3-f94e2efeba4b)



# RESULT:
The commands/batch files are executed successfully.


