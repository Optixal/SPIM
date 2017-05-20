# Shawn's Notes

## MAC Filtering
* Edit > Virtual Network Editor > Change Settings > Host only adapter > Uncheck DHCP service checkbox
* Record host only subnet
* Add a new host only adapter to server
* Change client's adapter to host only
* Rename server adapters to NAT and LAN respectively
* Change server's LAN IP to a valid IP in VMware's host only subnet, gateway (blank/placeholder), DNS 127.0.0.1
* Change server's NAT IP to a valid IP in VMware's NAT subnet, gateway VMware's gateway, DNS 127.0.0.1
* Set client's IP to auto, DNS to point to server's LAN IP
* Add new role: DNS
* Add new role: DHCP
* Add new role: Remote Access
  * Add role services: Routing
* Tools > Routing and Remote Access
* Right-click server > Configure and Enable Routing and Remote Access
  * Select 2nd option, NAT
  * Select NAT adapter
* Tools > DHCP
* Right-click IPv4 > New Scope
  * Enter DHCP lease range
  * Leave rest default
  * Click yes when asked whether to configure DHCP options now
  * Type server's IP for gateyway auto-assign and for DNS, leave WINS blank
  * Activate now
* Filters > Allow > New Filter > Enter MAC addr of client (use `ipconfig /all` on client to obtain MAC)
* Right-click DHCP server > All Tasks > Restart

## Links
* Windows 2012 Server Routing - http://www.dell.com/support/article/us/en/19/HOW10169/configuring-windows-server-2012-r2-as-a-router?lang=EN
* Windows 2012 DHCP Filters - https://technet.microsoft.com/en-us/library/ff521761.aspx
