![image](https://i.imgur.com/gBwrx1W.jpg)


<h1>Observing the Effect of a VPN on IP Addressing</h1>
In this short project, we will observe the impact of a virtual private network (VPN) on IP address, location, and web browsing. <br />

<h2>Environments and Technologies Used</h2>

-	ProtonVPN (free version)
- Microsoft Azure (Virtual Machines)
-	Remote Desktop


<h2>Operating System Used </h2>

- Windows 10 (21H2)

# Setting Up VPN in an Azure Virtual Machine

1. Go to "whatismyipaddress.com" on your actual PC. Take note of your public IP address and the city in a text file.

2. Create a [virtual machine](https://github.com/NicholasToon/Creating-Resource-Groups-and-Deploying-Virtual-Machines-in-Azure) in Azure and establish a connection to it using Remote Desktop Protocol (RDP).

3. Inside the Azure virtual machine, find the website "whatismyipaddress.com" again. Write down the new IP address and its location, which should *not* match your computer's IP address.

4. Download and install the ProtonVPN client. It will give you access to the free servers once you sign up and install the app.

5. Inside the VM, connect to a ProtonVPN server located in a country that is not your own. This establishes a VPN connection between the virtual machine and the chosen ProtonVPN server.

6. Go to "whatismyipaddress.com" using the Azure virtual machine while the VPN is on. Write down the new IP address and where it shows you are (like Naaldwijk, Netherlands), which should match the VPN server's location.

If everything went correctly, you will have three entries in your text file representing different IP addresses and locations:

 - IP address and location from your actual PC without using a VPN.

![image](https://i.imgur.com/TFS8VgX.png)

 - IP address and location from the Azure virtual machine without using a VPN.

![image](https://i.imgur.com/3HPgws4.png)

 - IP address and location from the Azure virtual machine with the VPN connected to a ProtonVPN server in the Netherlands.

![image](https://i.imgur.com/6XYoCAT.png)


## 

This exercise illustrates how VPNs work. VPNs encrypt and route your internet traffic through remote servers, creating a secure tunnel. This makes it seem as though you are browsing from various locations. VPNs can improve privacy and security and enable you to bypass geo-restrictions. However, it's important to note that using VPNs does not guarantee complete anonymity, regardless of any assurances provided in terms and conditions.
