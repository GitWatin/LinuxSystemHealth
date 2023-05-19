![header image](https://github.com/RIDWANE-EL-FILALI/LinuxSystemHealth/blob/fix_bugs/images/Untitled%20design.png)
<h1 align="center">
  🚀 Linux System Health 🖥️
</h1>

<p align="center">
  <a href="#">
    <img src="https://img.shields.io/github/license/GitWatin/LinuxSystemHealth" alt="Licence">
  </a>

  <a href="#">
    <img src="https://img.shields.io/github/v/release/GitWatin/LinuxSystemHealth" alt="Version">
  </a>

  <a href="https://www.paypal.me/valentindenis">
    <img src="https://img.shields.io/badge/Donate-PayPal-green.svg" alt="Donate">
  </a>
  
---
  
  
# INTRODUCTRION :
LinuxSystemHealth is a Bash script that provides an easy way to monitor and display essential system information at logon. It offers a comprehensive overview of the system's status, including CPU usage, memory usage, disk usage, network information, load averages, and service statuses.
By running this script upon logon, users can quickly assess the health and performance of their Linux systems. It is especially useful for system administrators and users who want to have a quick glance at their system's vital statistics without diving into complex monitoring tools.

Key Features:
- Displays the hostname, operating system, IP address, and other basic system information.
- Provides CPU usage percentage and the number of CPU cores.
- Shows load averages for 1-minute, 5-minute, and 15-minute intervals, indicating system load.
- Reports memory usage, including the total memory available and the amount in use.
- Monitors swap memory usage to assess virtual memory usage.
- Offers disk usage information for the root directory and, if present, the /share directory.
- Checks the status of essential services like SSH, Samba, Chronyd (NTP), SNMP, and FTP.

# USAGE :
Usage of the script is straightforward: simply run it upon logon to obtain an instant snapshot of your system's health. The output is neatly formatted and organized, making it easy to read and understand.
you can also use crontab to scechule the script to run every time the system boot's up
```
  1 - crontab -e
  2 - add the following line to the end of the file : @reboot /bin/bash /path/to/linuxsystemhealth.sh
```
# OUTPUT :
 ```
█=======================================================================
█    - Hostname....................: BROLY                          
█    - System......................: Kali GNU/Linux                            
█    - /Share......................: /share not found             
█    - /...........................: 18G / 192G       
█    - IP..........................: ***.***.***.***                                
█    ===================================================================
█    - CPU usage...................: 16.22%                       
█    - CPU Cores...................: 4                          
█    - Load........................: 0.94 - 0.73 - 0.75           
█    - Memory used.................: 4894 MB / 7369 MB        
█    - Swap in use.................: 550 MB / 28686MB MB      
█    ===================================================================
█    - SSH.........................: inactive                        
█    - Samba.......................: inactive                      
█    - Chronyd (NTP)...............: inactive                        
█    - NTP Synchronized............: inactive                             
█    - SNMP........................: inactive                       
█    - FTP.........................: inactive                        
█=======================================================================
```  
# NOTE :
The script includes support for CentOS, Debian, and Debian-based distributions like Ubuntu and Kali. It requires the "chronyd" package for CentOS.
  
# LICENSE :
LinuxSystemHealth is released under the MIT License, granting users the freedom to use, modify, and distribute the script according to their needs.




