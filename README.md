<h1>Setting up a Kali Linux Lab (VMWare)</h1>


<h2>Description</h2>
Project consists of setting up a Kali Linux Virtual Machine in VMWare.
<br/>

<h2>What I have Learned</h2>

- Adding a virtual machine image in VMware.
- Updating Kali Linux
- Upgrading installed packages in Kali Linux
- Securing Kali Linux
- Creating and managing permissions for a low level user

<h2>Languages and Utilities Used</h2>

<h3>Utilities</h3>

- VMware Workstation Player 17

<h3>Languages</h3>

- BASH

<h2>Environments Used </h2>

- Kali Linux

<h2>Prerequisites</h2>

- Internet Connection
- Kali Linux ios file
- VMware Workstation (VMware Workstation Pro is recommended, but I will use Workstation Player)

<h2>Steps taken:</h2>

<h3>Adding Kali Linux to VMware</h3>

- Downloaded the Kali Linux VMWare image from the Kali website and extracted the folder.
- After installing VMWare Player 17, clicked on <b>Open a Virtual Machine</b>
<img src='https://i.imgur.com/6ZzjkQY.png'>

- Find and open the Kali Linux VMWare virtual machine image from the extracted folder.
<img src='https://i.imgur.com/QMN2Ud6.png'>

VMware Workstation Player with the Kali Linux virtual machine.
<img src='https://i.imgur.com/LnxW6FQ.png'>

<h3>Kali Linux Hygiene</h3>

- Opening up the command line prompt, and running the command '<b>sudo apt update</b>' and enter the sudo password (the command is used for updating the OS) 
<img src='https://i.imgur.com/u9JOs37.png'>

- Run the command '<b>sudo apt upgrade -y</b>' to upgrade installed packages
<img src='https://i.imgur.com/Bpg7fpb.png'>

- Immediately run the command '<b>sudo apt autoremove</b>' to remove unwanted packages
<img src='https://i.imgur.com/H8o73xQ.png'>

<h3>Securing Kali</h3>

- Because the Kali Linux installed was preconfigured, change the password for the root user for the secure the virtual machine by using the command '<b>sudo su -</b>' to login as the root.
- Changing the password with the command '<b>passwd</b>'
<img src='https://i.imgur.com/9A3TUIN.png'>

- Add a new user by running the command '<b>adduser [username]</b>' followed by entering a secure password
 <img src='https://i.imgur.com/7jS9E9e.png'>

- After adding the low level user, add the sudo permission for root actions by running the command '<b>usermod -aG sudo [username]</b>'
- Following the command '<b>chsh -s /bin/bash [username]</b>' will make the low level user as the default user.
<img src='https://i.imgur.com/UGRnL0x.png'>

- Confirm that the new low level user has the sudo permission by running the command '<b>grep 'sudo' /etc/group</b>'

<h2>Resources Used</h2>

<h3>Youtube Videos</h3>

- <a href='https://www.youtube.com/watch?v=Vos7DCTqvSM'><b>Pro Tip: What to Do After Installing Kali Linux - Douglas | Cybersecurity</b></a>


<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
