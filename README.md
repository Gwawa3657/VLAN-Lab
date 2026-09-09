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
<img width="688" height="698" alt="Screenshot 2026-09-08 183934" src="https://github.com/user-attachments/assets/321ededf-365b-4a01-bf3d-373f9299fa81" />
<img width="690" height="697" alt="Screenshot 2026-09-08 183830" src="https://github.com/user-attachments/assets/afc6eff8-48de-4c25-bd35-303b4d22197f" />


