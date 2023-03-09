# Windows-Forensics-Notes

## Table of Contents

| Table of Contents |
| -------------------- |
|  | 
|  |
|  |


## Windows Acquisition

+ FTK Imager
+ KAPE
+ WinTriage



SAM (mounted on HKEY_LOCAL_MACHINE\SAM) > users info and grops

VPN connection > \Software\Microsoft\Windows NT\CurrentVersion\NetworkList

Windows shares > SYSTEM\CurrentControlSet\Services\LanmanServer\Shares

settings for IP Address > HKLM\SYSTEM\CurrentControlSet\Services\Tcpip\Parameters\Interfaces

Run command history > HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Explorer\RunMRU




| Registry keys | Description |
| -------------------- | -------------------- |
| HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\Session Manager\Memory Management | contains information about memory management settings on the system |
| HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\Session Manager\Environment  | contains environment variables that are set on the system |
| HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\ProfileList | contains information about the user profiles that are configured on the system |
| HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Services | contains information about the services that are installed on the system |
| HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\ComputerName | contains information about the computer name and domain membership |
| HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\TimeZoneInformation | contains information about the time zone settings on the system |
| HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\Windows | contains information about the system's graphical user interface (GUI) settings, including the desktop background and screen saver |
| HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\FontSubstitutes | contains information about font substitutions on the system |
| HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Explorer\Shell Folders | contains information about the locations of various system folders, such as the desktop and the Start menu |
| HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Services\Tcpip\Parameters | contains information about the system's TCP/IP settings, such as the IP address and subnet mask |
| HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Run | contains a list of programs that are automatically started when the system boots up |
| HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Policies\System | contains information about system policies that are enforced on the system |
| HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Policies\Explorer | contains information about Explorer policies that are enforced on the system |
| HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Enum | contains information about hardware devices that are installed on the system |
| HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Services\Winsock2\Parameters | contains information about the system's Winsock settings, which are used for network communication |
| HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Internet Settings | contains information about the system's Internet settings, including the browser history and cookies |
| HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Explorer\RecentDocs | contains information about recently opened documents |
| HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\Drivers32 | contains information about audio drivers on the system |
| HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\Print\Printers | contains information about installed printers on the system |


## Command

systeminfo : information about machine
net user : users in system
net user ahmed : info about Ahmed


## Paths

C:\Windows\System32\Tasks : Scheduled Tasks Path

hosts file path : C:\Windows\System32\Drivers\etc\hosts

---------------------------------
