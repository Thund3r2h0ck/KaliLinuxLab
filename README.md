<h1>Setting up a Kali Linux Lab (VMWare)</h1>


<h2>Description</h2>
Project consists of setting up a Kali Linux Virtual Machine in VMWare.
<br/>

<h2>What I have Learned</h2>

- Adding a virtual machine image in VMware.
- Updating Kali Linux
- Upgrading installed packages in Kali Linux

<h2>Languages and Utilities Used</h2>

- VMware Workstation Player 17

<h2>Environments Used </h2>

- Kali Linux

<h2>Prerequisites</h2>

- Internet Connection
- Kali Linux ios file
- VMware Workstation (VMware Workstation Pro is recommended, but I will use Workstation Player)

<h2>Steps taken:</h2>

<h3>Adding Kali Linux to VMware</h3>

- I downloaded Kali Linux VMWare image from the Kali website and extracted the folder.
- After installing VMWare Player 17 to my PC, I clicked on <b>Open a Virtual Machine</b>
<img src='https://i.imgur.com/6ZzjkQY.png'>

- Find and open the Kali Linux VMWare virtual machine image from the extracted folder.
<img src='https://i.imgur.com/QMN2Ud6.png'>

VMware Workstation Player with the Kali Linux virtual machine.
<img src='https://i.imgur.com/LnxW6FQ.png'>

<h3>Kali Linux Hygiene</h3>

- Opening up the command line prompt, and running the command '<b>sudo apt update</b>' and enter the sudo password (the command is used for updating the OS) 
<img src='https://i.imgur.com/u9JOs37.png'>

- Running the command '<b>sudo apt upgrade -y</b>' to upgrade installed packages
<img src='https://i.imgur.com/Bpg7fpb.png'>

- Immediately run the command '<b>sudo apt autoremove</b>' to remove unwanted packages
<img src='https://i.imgur.com/H8o73xQ.png'>


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
