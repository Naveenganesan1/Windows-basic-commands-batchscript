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

![330012900-c65ec521-e638-4a1f-8bdd-97c56e1efc85](https://github.com/user-attachments/assets/11c78cfc-871d-42bc-a4cb-601766ee387b)



Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
```
cd %userprofile%\Desktop\MyLab
```
![330013412-b9be78f6-9828-4e71-a5a9-f6f1189783ed](https://github.com/user-attachments/assets/800bdcc4-f13c-421a-b084-6f004c4416f1)
```
type nul > MyFile.txt
```

![330013653-bd325e68-6b4b-4534-8545-4a27ff88884b](https://github.com/user-attachments/assets/efcb5f41-93b4-48d3-9a8d-f1c140eb39ac)



List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
```
dir %userprofile%\Desktop\MyLab
```

![330012712-30682b3a-8a3a-42f2-a0ce-4e01779085c9](https://github.com/user-attachments/assets/7bd7c18b-3a0f-46d1-a033-561a38eef4d9)




Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Backup
```

![330012322-64b3d1fb-6b15-47d7-b449-18d1df73456e](https://github.com/user-attachments/assets/4509d3e5-08ac-4217-9db5-0adbb71c4491)
```
copy MyFile.txt %userprofile%\Desktop\Backup
```

![330012410-6a48ce78-88e9-4a7e-a2e5-8ece42f7311e](https://github.com/user-attachments/assets/f3e23263-e0ab-4117-b517-dee3301a57e7)


Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Documents
move MyLab Documents
```

![330012125-1b3b3dfc-19ad-4574-98e2-e28bd46533f1](https://github.com/user-attachments/assets/5b659bf2-ede0-428d-811f-a47500bfec7a)



## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

 ## COMMAND
 ```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```

![330011170-759f68b0-4717-4bea-9e37-4f8bc436e3b6](https://github.com/user-attachments/assets/6c321598-bdec-496a-bcbe-a2ed419dc95f)


 ## COMMAND
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```

 


## OUTPUT


![330011376-c3bd3e5a-2d4b-4db4-b681-8557bc05d5c6](https://github.com/user-attachments/assets/46222b08-27be-4efa-90fe-f244354890da)



# RESULT:
The commands/batch files are executed successfully.

