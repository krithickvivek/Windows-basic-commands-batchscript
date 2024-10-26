# Windows-basic-commands-batchscript
Ex08 - Windows-basic-commands-batchscript

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

## COMMAND AND OUTPUT:
Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.

```
mkdir %userprofile%\Desktop\MyLab
```

![image](https://github.com/user-attachments/assets/0edd8aeb-65f5-4638-8f2d-e02d831c8129)

## COMMAND AND OUTPUT:
List the contents of the "MyLab" directory.

```
cd %userprofile%\Desktop\MyLab
```

![image](https://github.com/user-attachments/assets/8771eeaa-d1e0-46e2-a3db-ae6687f5d6d9)

![image](https://github.com/user-attachments/assets/05283b9e-93ab-4b33-8d9e-1d407cd71939)

## COMMAND AND OUTPUT:
Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

```
dir %userprofile%\Desktop\MyLab
```

![image](https://github.com/user-attachments/assets/afcebb38-ce57-469a-ba0f-6e70f8b46843)

## COMMAND AND OUTPUT:
Move the "MyLab" directory to the "Documents" folder.

```
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup
```

![image](https://github.com/user-attachments/assets/51e9371f-efa5-4297-a600-a40ba3715254)

![image](https://github.com/user-attachments/assets/7212927c-ce58-4362-a40f-f64abd6accd3)

## COMMAND AND OUTPUT:
```
mv Myfile.txt %userprofile%\Documents
```

![image](https://github.com/user-attachments/assets/9243a9c1-9414-4907-a32e-352a72ee283b)

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

## OUTPUT:
![image](https://github.com/user-attachments/assets/68ca1a48-958d-4d67-a7d4-29256d7e2bc6)

# RESULT:
The commands/batch files are executed successfully.

