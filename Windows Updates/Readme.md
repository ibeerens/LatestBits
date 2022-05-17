**Windows Updates examples**

*PSWindowsUpdate*
Set-ExecutionPolicy -ExecutionPolicy Unrestricted

PSWindowsUpdate
Install-Module PSWindowsUpdate

Import-Module PSWindowsUpdate
Get-WindowsUpdate

Install-WindowsUpdate

The above mentioned command will only install Windows updates. If you want to update other Microsoft products as well, you’ll need to enable the Microsoft Update Service as well. It’s pretty easy to enable it using PowerShell:

Add-WUServiceManager -MicrosoftUpdate


*Windowss Update command*
wuauclt /detectnow /updatenow

*Windows 10/Server 2016 commmand*
UsoClient.exe /StartScan

Options:
/StartScan, /StartDownload, /StartInstall


