Section C. Forensic Script Details [!!!AV/EDR/EPP whitelisting is required prior to execution!!!]: Please run the script from the respective SFTP site of your office only.

 Forensic script [for Windows 7+ and windows 2008 R2+ 64bit systems]:

 

1.    The forensic script is placed on the outgoing\ForensicScript folder of the sftp called “forensic_collector_<client name>_64.exe" 

Compatibility: 64bit sensor: Windows7+, Windows 2008 R2+ systems

Please ensure to run the script as admin

2.    Once the script is run it will take around 10 to 15 minutes to finish, it will collect data at C:\windows\temp\COMPUTERNAME-IR folder and in the end creates a COMPUTERNAME.IZE file in the folder.

3.    Please collect the folder manually and upload to incoming folder of the sftp if the system is offline.

4.    If the system is online we should automatically receive it to our cloud.

5.    Please make sure CRA received the forensic script or collect the output manually before any restore.

 

Forensic script for legacy systems [windows 2008 non r2, Windows 2003 and windows XP or any 32 bit systems]:

 

For systems not compatible, you can run the legacy forensic script in the outgoing\Forensic Script\legacy folder called "forensic_collector_legacy_*.exe" folder.

This script takes longer to run around 30minutes on the system. Once done it will Create a *.ize file on C:\

[Note: if after 30min if you don’t see a .ize file on C:\, please copy the "C:\inspect" folder, rename it with system name and upload to the SFTP]

Note: The scripts will run silently on the system. Please do run it as admin.

 

Please whitelist 3.13.41.208 over port 22 for our forensic scripts to reach out back to our cloud.

 

Below are some apps which might be seen on the system when running the forensic script.

 

c:\windows\temp\<ComputerName>_ir\data\ir_arn.exe

c:\windows\temp\<ComputerName>_ir\data\ir_tcon.exe

c:\windows\temp\<ComputerName>_ir\data\ir_lsess.exe 

 