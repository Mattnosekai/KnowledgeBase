#Find Internal/Local IP Address on Windows.

At the command prompt type **ipconfig**

#Find External/Public  IP Address on Windows.
 

At the command prompt type **nslookup myip.opendns.com resolver1.opendns.com**

In Powershell **(Invoke-WebRequest ifconfig.me/ip).Content.Trim()**
 

#Copy a Directory and its Structure on Windows.

At the command prompt type **Robocopy /S /E  source_full_path  destination_full_path**
 

#Copy a File on Windows.

At the command prompt type **copy source_directory\filename**
(to copy to the current directory)

At the command prompt type **copy source_directory\filename  destination_directory\filename**


#Get the Hostname on Windows.

At the command prompt type **hostname**

At the command prompt type **ipconfig /all**

 
#Get the MAC/Physical Address on Windows.

This is the address of the NIC or Wireless card.

At the command prompt type **getmac /s localhost**

At the command prompt type **ipconfig /all**


#Find if System is 32-Bit or 64-Bit..etc on Windows.


At the command prompt type **wmic os get osarchitecture**
 

#Find System Specs on Windows.

At the command prompt type **start control system**
 

#Find Disk Space on Windows.

At the command prompt type **start system**

then open Computer or This PC folder to see disk space
 

#Get OS Version on Windows.


At the command prompt type **winver**
 

#Find if an Internet Connection is available on Windows.
 

At the command prompt type **ping www.google.com**

If a connection is available then it will show 0% packet loss.

 

#Kill a Program or Process in Windows.

At the command prompt type **taskkill /f /im exename* /t**
Can be a partial name when wildcard is used.
 

#Restart the Computer on Windows.

At the command prompt type **shutdown /r**


#Shutdown the Computer on Windows.


At the command prompt type **shutdown /s**


#Delete a Directory and sub-directories on Windows.

At the command prompt type **rmdir /q /s directoryname**


#Make a Directory on Windows.
 

At the command prompt type **mkdir directoryname**


#Find any File by Name on Windows.

At the command prompt type **where /r c:\ filename >outputfile.txt**
(wildcards * can be used for both the filename and extension)


#Search All Files for String on Windows.

In Powershell type:
**get-childitem c:\ *.txt –rec|select-string “youtube” –list|Select Path|out-file output.txt**
(This will search all files with a .txt extension for the string “youtube” and output the path and
Filename to output.txt)
