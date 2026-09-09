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
<p align="left">
<img width="681" height="658" alt="Screenshot 2026-09-08 214527" src="https://github.com/user-attachments/assets/2c824ecc-9de8-4d2f-820f-478eceee355b" />
</p>
<br> PC0 and Laptop1 are connected to interface 0/2 and 0/3
<br> the command "interface fastethernet" changes which interface is being configured.
<br> "switchport mode access" > "switchport access vlan 2 will put the computer connected to that interface into the vlan 2 I created
<p align="left">
<img width="312" height="123" alt="Screenshot 2026-09-08 215558" src="https://github.com/user-attachments/assets/ce6ddad8-5826-49be-aca8-56ccd17bb22e" />
</p>
<br> To make sure these computers are segmented properly I access the command prompt in PC0 and try to ping PC2 which is not in our VLAN.
<br> The ping returns a Request timed out which means it was set up properly.
<p align="left">
<img width="1146" height="181" alt="Screenshot 2026-09-08 220636" src="https://github.com/user-attachments/assets/402df7e1-7dc9-48df-9713-de7863e98277" />
</p>
<br> PC2 and PC3 are are connected to interface 0/4 and 0/5
<br> PC4 and Laptop0 are connected to interface 0/6 and 0/7
<br> Once again go into the network switch config and switch PC2 and PC3 to vlan 3
<br> Switch PC4 and Laptop0 to vlan 4
<p align="left">
<img width="685" height="692" alt="Screenshot 2026-09-08 221520" src="https://github.com/user-attachments/assets/b625c7fc-e28c-4a26-808f-3dbc0e95308a" />
</p>
<br> The devices can now only talk to each other if they are in the same VLAN.
<br> Can test this anytime by going into the command prompt in one pc and trying to ping another that's in a different VLAN. (EX. PC2 to PC4)
<p align="left">
<img width="689" height="700" alt="Screenshot 2026-09-08 221900" src="https://github.com/user-attachments/assets/377516ed-6ab4-4663-9e1f-db154f07012f" />
<img width="806" height="576" alt="Screenshot 2026-09-08 221907" src="https://github.com/user-attachments/assets/b7fa4914-e97f-4144-a101-1a37ccf2224d" />
</p>
