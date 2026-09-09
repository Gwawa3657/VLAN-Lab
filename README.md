# VLAN-Lab

## Objective
Last time i used Cisco Packet Tracer was when I was studying for the Network+ I wanted to refresh my memory on how to set up small networks. I thought I would practice with configuring VLANs. I tried it with my home network and although I succeeded, it was a mess.

<br> Setup a Router, Switch, and 6 devices.
<br> Connect everything with Copper-Straight through cables. I used FastEthernet Interfaces 1-7
<br> The router will be down so click on it and go to CLI and type no.
<br> Enter these commands:
<br> en (enable configuration)
<br> conf t (Configure Terminal)
<br> interface gigabitEthernet 0/0
<br> ip address 192.168.1.1 255.255.255.0
<br> no shutdown
<img width="1327" height="707" alt="Screenshot 2026-09-08 181455" src="https://github.com/user-attachments/assets/22d19f31-0382-4a30-8ae4-95a8f8fe7d2d" />
<br> Go into each PC or device then Desktop > IP Configuration
<br> Change the Default Gateway to 192.168.1.1
<br> IPv4 Address will be 192.168.1.10 For every device after the scheme is .20 .30 .40 etc.
<img width="690" height="697" alt="Screenshot 2026-09-08 183830" src="https://github.com/user-attachments/assets/aba99f91-77ab-4672-bdc9-82d75c18c8bd" />
<img width="688" height="698" alt="Screenshot 2026-09-08 183934" src="https://github.com/user-attachments/assets/11f443f3-ee2e-4e45-8ed9-88725f6cff07" />
<br> Click on a PC then Desktop > Command Prompt 
<br> I needed to check if there was connectivity so I pinged another device.
<img width="687" height="680" alt="Screenshot 2026-09-08 184154" src="https://github.com/user-attachments/assets/32a87dc6-07de-4d45-8859-56a9070d6ad7" />
<br> I went into the the switch interface to configure the VLANs
<br> VLAN1 is the default so it's name can't be changed.
<br> I made 3 VLANs and named them 2 3 and 4
<img width="681" height="658" alt="Screenshot 2026-09-08 214527" src="https://github.com/user-attachments/assets/2c824ecc-9de8-4d2f-820f-478eceee355b" />

