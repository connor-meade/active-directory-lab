## Simulated Active Directory environment using Windows Server 2022 and VirtualBox.


### Steps Taken:
* Promoted Server to Domain Controller.

* Configured a dual-NIC setup to separate internet access (NAT) from internal domain traffic using a private subnet (172.168.0.0/24), ensuring secure and isolated domain communication.

* Created an administrative OU and a user account, assigned the account Domain Admin rights.

* Configured Routing and Remote Access Service (RRAS) to provide NAT-based internet access for the internal network.

* Implemented DNS and DHCP services to facilitate domain name resolution and dynamic IP addressing within the internal network, including creating and configuring a DHCP scope. Enabled routing via RRAS to support network traffic flow.
  
* Automated user account creation by running a PowerShell script to import entries from a names.txt file into Active Directory, including initial password setup.

* Provisioned a Windows 11 virtual machine, joined it to the domain, and verified DNS functionality and network connectivity using command-line tools such as ping.
