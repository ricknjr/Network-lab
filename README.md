# Network-lab
My small business network created in GNS3
![Stage0-network-topology](https://github.com/ricknjr/Network-lab/assets/160628458/fff75c90-fa9f-4611-a7e2-5d39b02bf589)

During this process I added a new device (Win10) and linked them up. When adding Win10 I had to set up IP ranges, set up a gate way and a DHCP server.LAN and firewall were configure through CLI over interface (10.128.10.1) This was done by setting the allowaccess and also the DHCP sever was enable on the LAN interface.Win10 was added to LAN network.

![Stage2-network-topology](https://github.com/ricknjr/Network-lab/assets/160628458/cc2051ff-be10-4387-bec7-3c5843d5f7f5)
In this process i was asked to add a new device to the worspace and linked them up as shown in stage01. In this server i had to set up an "Active Directory Domain Services" server role.First I had to prepared the Win2012r2 server for the "Active Directory Services." I did this by setting up an ip address, subnet mask, dafault gateway, DNS1 and DNS2 on the internet Protocol Version 4.I also synchronized the time with the internet server to 10.128.0.1.Once this was done I continued to set up the Active Directory Domain Services.This was done by following the learn.microsoft.com steps that it gives out.Once the Active Directory Domain was created I created users for the Active Directory to become Domain Admins. Next I prepared Win10 to join the server. Later I set up a group policy to for a background.
