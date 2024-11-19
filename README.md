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

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.

```
mkdir %userprofile%\Desktop\MyLab
```
![384053505-a59bf44e-16af-4a90-a0d7-098fbab12551](https://github.com/user-attachments/assets/6fb1025e-fd54-41e0-9176-b110a1532646)

## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.
```
cd %userprofile%\Desktop\MyLab
```
![384053629-fa8813c6-feeb-415e-93cf-7677f0df6856](https://github.com/user-attachments/assets/b3ca7f84-d9af-4895-a288-7d2c9b43b244)

![384053689-4ecc883b-02f1-49cb-ad4d-8c0437f99c21](https://github.com/user-attachments/assets/06a8013b-5603-4707-a862-454dd2ff8439)

## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
```
dir %userprofile%\Desktop\MyLab
```
![384054529-91e0cf60-fdf3-4987-8d73-48f4111271c5](https://github.com/user-attachments/assets/5fe1ef14-8037-487b-8386-daeb3dcde131)

## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.
```
mkdir %userprofile%\Desktop\Backup
copy MyFile.txt %userprofile%\Desktop\Backup
```
![384054671-156d4423-4163-4d7f-bbeb-ea8ec1dde82e](https://github.com/user-attachments/assets/aa956e22-0232-43da-92ed-784e04525453)

![384054697-bd25177f-3a51-4a6b-8a09-e1d243f818eb](https://github.com/user-attachments/assets/b3959179-2a5e-4522-9f04-a9b6fc18aa69)

## COMMAND AND OUTPUT
```
mv Myfile.txt %userprofile%\Documents
```
![384054823-22b175a0-8b2e-4085-9b6d-1dde324c7e2f](https://github.com/user-attachments/assets/1fa5b3a3-e831-4328-aafb-e6710e16d678)

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

![384055188-e58fad14-1744-48d2-a5f3-7f8d59c420fb](https://github.com/user-attachments/assets/07fb754b-e347-4ec2-82bd-82ab9af10dc0)


# RESULT:
The commands/batch files are executed successfully.

