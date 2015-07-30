# SSD
I got an SSD, what should I remember to do ?

* Change the location of music, videos, pictures (in W10 system menu)
* Remove the page file
* Change Appdata folder location to HDD (I do not, for speed)
* Change Temp folder location to HDD (Environnement variable to `D:\Temp\User` and `D:\Temp\System`)
* Enable AHCI
* Enable TRIM (`fsutil behavior set disabledeletenotify 0`)
* Disable system restore
* Disable indexing on SSD
* Disable Hibernation ( `powercfg -h off` )
* Disable Prefetch & Superfetch ( `HKEY_LOCAL_MACHINE\CurrentControlSet\Control\SessionManager\Memory Management\PrefetchParameters`)
* Disable services for Windows Search and Superfetch
* Disable ClearPageFileAtShutdown and LargeSystemCache ( `HKEY_LOCAL_MACHINE\CurrentControlSet\Control\SessionManager\Memory Management` )