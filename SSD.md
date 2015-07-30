# SSD
I got an SSD, what should I remember to do ?

* Change the location of music, videos, pictures (in W10 system menu)
* Change Appdata folder location to HDD (I do not, for speed)
* Change Temp folder location to HDD (Environnement variable to `D:\Temp\User` and `D:\Temp\System`)
* Enable AHCI
* Enable TRIM (`fsutil behavior set disabledeletenotify 0`)
* Disable system restore
* Disable indexing on SSD, [Move index folder to HDD](http://windows.microsoft.com/fr-be/windows7/change-advanced-indexing-options)
* Disable Hibernation ( `powercfg -h off` )
* Disable Prefetch & Superfetch ( `HKEY_LOCAL_MACHINE\CurrentControlSet\Control\SessionManager\Memory Management\PrefetchParameters`)
* Disable service for Superfetch ( `services.msc` )
* Disable ClearPageFileAtShutdown and LargeSystemCache ( `HKEY_LOCAL_MACHINE\CurrentControlSet\Control\SessionManager\Memory Management` )

### Source

https://www.maketecheasier.com/12-things-you-must-do-when-running-a-solid-state-drive-in-windows-7/