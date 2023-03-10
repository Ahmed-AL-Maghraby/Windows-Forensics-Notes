
 | Table of Contents |
 | ----------------- |
 | [Windows Prefetch files](https://github.com/ahmed-kamal-el-maghraby/Windows-Forensics-Notes/blob/main/Windows%20Disk%20Forensics.md#windows-prefetch-files) |
 | [Windows 10 Timeline](https://github.com/ahmed-kamal-el-maghraby/Windows-Forensics-Notes/blob/main/Windows%20Disk%20Forensics.md#windows-10-timeline) |
 | [Windows Jump Lists](https://github.com/ahmed-kamal-el-maghraby/Windows-Forensics-Notes/blob/main/Windows%20Disk%20Forensics.md#windows-jump-lists) |
 | [Shortcut Files](https://github.com/ahmed-kamal-el-maghraby/Windows-Forensics-Notes/blob/main/Windows%20Disk%20Forensics.md#shortcut-files) |
 | [IE/Edge history](https://github.com/ahmed-kamal-el-maghraby/Windows-Forensics-Notes/blob/main/Windows%20Disk%20Forensics.md#ieedge-history) |
 | [Setupapi dev logs for USB devices](https://github.com/ahmed-kamal-el-maghraby/Windows-Forensics-Notes/blob/main/Windows%20Disk%20Forensics.md#setupapi-dev-logs-for-usb-devices) |
 
 ## Windows Prefetch files

When a program is run in Windows, it stores its information for future use. This stored information is used to load the program quickly in case of frequent use. This information is stored in prefetch files which


+ ### Path :
  -  `` C:\Windows\Prefetch directory``

- Prefetch files have an extension of .pf
- contain the last run times of the application
- the number of times the application was run
- and any files and device handles used by the file


<br> 

 ## Windows 10 Timeline

Windows 10 stores recently used applications and files in an SQLite database called the Windows 10 Timelineand It contains the application that was executed and the focus time of the application.



+ ### Path :
  -  `` C:\Users\<username>\AppData\Local\ConnectedDevicesPlatform\{randomfolder}\ActivitiesCache.db ``


<br> 

 ## Windows Jump Lists

Windows introduced jump lists to help users go directly to their recently used files from the taskbar. We can view jumplists by right-clicking an application's icon in the taskbar, and it will show us the recently opened files in that application.

 include information about the applications executed, first time of execution, and last time of execution of the application against an AppID


+ ### Path :
  -  `` C:\Users\<username>\AppData\Roaming\Microsoft\Windows\Recent\AutomaticDestinations ``




<br> 

 ## Shortcut Files


Windows creates a shortcut file for each file opened either locally or remotely. The shortcut files contain information about the first and last opened times of the file and the path of the opened file, along with some other data. Shortcut files can be found in the following locations:

provide us with information about connected USB devices. It can provide us with information about the volume name, type, and serial number. 



+ ### Path :
  -  `` C:\Users\<username>\AppData\Roaming\Microsoft\Windows\Recent\ ``
  - `` C:\Users\<username>\AppData\Roaming\Microsoft\Office\Recent\ ``

The creation date of the shortcut file points to the date/time when the file was first opened. The date/time of modification of the shortcut file points to the last time the file was accessed.




<br> 

 ## IE/Edge history

An interesting thing about the IE/Edge browsing history is that it includes files opened in the system as well, whether those files were opened using the browser or not. Hence, a valuable source of information on opened files in a system is the IE/Edge history.



+ ### Path :
  -  `` C:\Users\<username>\AppData\Local\Microsoft\Windows\WebCache\WebCacheV*.dat ``



<br> 

 ## Setupapi dev logs for USB devices

When any new device is attached to a system, information related to the setup of that device is stored in the setupapi.dev.log.



+ ### Path :
  -  `` C:\Windows\inf\setupapi.dev.log ``

This log contains the device serial number and the first/last times when the device was connected. 

