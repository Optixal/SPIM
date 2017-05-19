# SPIM

## Setup Steps (Done)
* [x] Start Win 2012 Server
* [x] Set IP to static
* [x] DNS to 127.0.0.1
* [x] Gateway to 192.168.137.1
* [x] Add roles and features
* [x] Select both Active Directory and DNS Services
* [x] Keep default features
* [x] Promote to DC
* [x] Add new forest
* [x] Enter domain name like "www.let.com"
* [x] Enter DSRM password of "1qwer$#@!"
* [x] Enter NetBIOS name of "LET_DC"
* [x] Continue rest with defaults
* [x] Wait for install and restart
* [x] Reset pass to "1qwert%$#@!"
* [x] On host, bridge wifi to ethernet
* [x] Ethernet shud by default be 192.168.137.1
* [x] In VMware modify Virtual Network Adapter, bridge to ethernet
* [x] Change the server's VMware adapter to bridged

## Informational
* [ ] When presenting, present 2 workstations (one with daz and one without) and the server.
* [ ] The office is just a room small, consisting only of workstations, all connected properly already, low budget for physical security CCTV (at the door) and card access
* [ ] Cameras - let them bring in

## Custom Requests
* [ ] Internet access office all workstations - university's network lan cable, not wireless
* [ ] Ppl cant plug anything into the lan cable - prob mac filtering (Shawn)
* [ ] Caught locally storing data, will be scolded
* [x] Try not to let users save stuff locally (Aloysius) (http://www.windowsnetworking.com/kbase/WindowsTips/Windows2003/AdminTips/Admin/SettingUpDiskQuotaswithGroupPolicy.html)
* [ ] Physical policy - no personal keyboards, mouse, usb hard drive, esp those with on-board-storage, no personal usb peripherals
* [x] Prevent usb from connecting / read write (Aloysius) (https://support.microsoft.com/en-us/help/555324)
* [x] Passwords should be allowed to be changed to be users - after expiry (90 days mentioned below) will lock out user. Send reminder maybe a week before (Elroy)
* [ ] Personal devices allowed inside - signed NDA (prob policy)
* [ ] Prob have firewall block all, no remote access, no port opens
* [ ] Admins must be able to login with the same password

## OS and Applications
* [ ] OS: Windows 10 
* [ ] AVG anti-virus (http://www.avg.com/ww-en/homepage)
* [ ] Internet Explorer 11
* [ ] Java SE 8 Update 65 or higher higher (http://www.oracle.com/technetwork/java/javase/downloads/index-jsp-138363.html)
* [ ] Open Office (https://www.openoffice.org/download/index.html)
* [ ] Adobe Acrobat (https://get.adobe.com/reader/)
* [ ] Adobe Flash (https://get.adobe.com/flashplayer/)
* [ ] DAZ Studio (Evaluation) (On 1 workstation only) (https://www.daz3d.com/get_studio)
 
## LET Image 
* [ ] All workstations connecting to network are required to display the following image before the login screen:
* [ ] LET Image will be reviewed by management periodically. You can download this from Blackboard > SPIM>Module Assessment.

## Workstation security configuration
* [ ] All LET workstations will have an administrative account;
* [ ] Only the LIC and PO will have Administrator level access to workstations (Wen Jun)
* [ ] Periodic reviews of Administrator group membership will be performed;
* [ ] Workstations are locked down to prevent software installation or configuration modification by anyone other than the LIC or PO (Wen Jun)
* [ ] Workstation names should follow the naming convention of LET-# asset tag (eg. 13573) (gonna do on Win10)
* [ ] At least once a year, the workstation inventory information should be reviewed and updated for all workstations;
* [ ] Periodic audits of workstations will be conducted to ensure that they remain in compliance; and
* [ ] Any deviations from the approved configuration discovered in any audit must be corrected immediately.

## Domain Password Policy

### The workstation password must: (Elroy)
* [x] be made up of a minimum of eight alphanumeric characters, containing at least one letter and one numeral;
* [x] be changed at least every 90 days;
* [x] not be reused for at least three generations of password;
* [ ] not be displayed in clear;
* [x] be locked out at a maximum of three failed attempts;
* [x] be changed upon the first login; and
* [ ] not be the same as the account ID or user ID.
 
## Software Purchase and Installation
* [ ] All software to be installed on workstations must be acquired through the LIC.
* [ ] PO will manage centrally licensed software such as email, anti-virus, and application software.

## Data storage
* [ ] Important files should be stored on a network server in the appropriate file share and not on the workstation.
* [ ] Workstations are not backed up and are subject to re-image; therefore there is no guarantee that data stored on the workstation will be recovered in the event of system problems, loss or theft.
