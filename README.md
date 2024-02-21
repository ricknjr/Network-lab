# Network-lab
My small business network created in GNS3
![Stage0-network-topology](https://github.com/ricknjr/Network-lab/assets/160628458/fff75c90-fa9f-4611-a7e2-5d39b02bf589)
---
During this process I added a new device (Win10) and linked them up. When adding Win10 I had to set up IP ranges, set up a gate way and a DHCP server.LAN and firewall were configure through CLI over interface (10.128.10.1) This was done by setting the allowaccess and also the DHCP sever was enable on the LAN interface.Win10 was added to LAN network.
![Stage1-network-topology](https://github.com/ricknjr/Network-lab/assets/160628458/272fadeb-ce96-4f55-af32-99d67b1a94f7)
---
In this process i was asked to add a new device to the worspace and linked them up as shown in stage01. In this server i had to set up an "Active Directory Domain Services" server role.First I had to prepared the Win2012r2 server for the "Active Directory Services." I did this by setting up an ip address, subnet mask, dafault gateway, DNS1 and DNS2 on the internet Protocol Version 4.I also synchronized the time with the internet server to 10.128.0.1.Once this was done I continued to set up the Active Directory Domain Services.This was done by following the learn.microsoft.com steps that it gives out.Once the Active Directory Domain was created I created users for the Active Directory to become Domain Admins. Next I prepared Win10 to join the server. Later I set up a group policy to for a background.
![Stage2-network-topology](https://github.com/ricknjr/Network-lab/assets/160628458/cc2051ff-be10-4387-bec7-3c5843d5f7f5)
---
![Stage3-network-topology](https://github.com/ricknjr/Network-lab/assets/160628458/f4e5a979-5a00-422b-8538-907b60ae4078)

Here i added Win2012r2 server to join the domain.This was done by giving it the static ip address of 10.128.0.80 and also setting up the primary DNS ip from the preivious server as a primary  and the Firewall LAN IP as a secondary. At the end everything was sync with dc.widgets.localdomain.Once the server has joined the the domain i installed the Internet Information Services.I ended up creating a test webpage on IIS and made sure it was able to be access by win10 workstation.
