# Disk Space Reporting Script (Powershell & HTML) #

This is a Powershell script to report on a list of server's disks space.  Unlike most reports out there, this one only reports on those disks that are below the set thresholds. The HTML report is embedded in the body of the email so no one will have to open an ugly CSV file.


 ![](Images/HTMLReport.png?raw=true)
 
 
## Highlights ##


* Checks disk space and sends an HTML report as the body of an email 
* Reports only disks on computers that have low disk space. (Can be changed to send a report regardless)
* Thresholds can be set as required
* Emails can be sent to individuals and / or distribution lists
* Built-In cleanup of old files. Defaults to 7 days of reports but can be amended (Ensure this is placed in a location other than where the script is stored, otherwise it will delete the script)
* Separate text document used to list servers / desktops


## Usage ##


All environmental variables are self-explanatory in the script. If you wish for the report to send even when a threshold hasn't been triggered, just change the following:

Currently: $i -gt 0
Change to: $i -ge 0


 ## Requirements ##

 
**Computer Targets** (Server or Desktop)

* Active Directory domain membership
* Supported Operating Systems
 * Windows Server 2012
 * Windows Server 2012 R2
 * Windows Server 2008 R2
 * Windows Server 2008
 * Windows Server 2003
 * Windows 7
 * Windows XP
 * Windows 2000

<br>
<br>
<br>
<br>
<br>

###### Special Thanks ######

<br>
<br>
<br>
_Mike Carmody_
_Thiyagu_
