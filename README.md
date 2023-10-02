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

## Exercise Procedure 

1. Go to "whatismyipaddress.com" on your actual PC. Take note of your public IP address and the city.

2. Create a <a href="https://github.com/NicholasToon/Creating-Resource-Groups-and-Deploying-Virtual-Machines-in-Azure" virtual machine> in Azure and establish a connection to it using Remote Desktop Protocol (RDP).

3. Inside the Azure virtual machine find the website "whatismyipaddress.com" again. Write down the new IP address and its location, which should not match your computer's IP address.

4. Download and install the ProtonVPN client. It will give you access to the free servers once you sign up and install the app.

5. Inside the VM, connect to a ProtonVPN server located in a country that is not your own. This establishes a VPN connection between the virtual machine and the chosen ProtonVPN server.

6. Access the website "whatismyipaddress.com" again from within the Azure virtual machine, with the VPN active. Take note of the new IP address and location displayed. This IP address should reflect the location of the VPN server (e.g., Tokyo, Japan).

By following these steps, you will have three entries in your text file representing different IP addresses and locations:

1. IP address and location from your actual PC without using a VPN.

![image](https://i.imgur.com/TFS8VgX.png)

4. IP address and location from the Azure virtual machine without using a VPN.

![image](https://github.com/JasonDelahoussaye/Virtual_Private_Network_VPN_IP_Address_Observations/assets/106440235/0ffe175a-a0f2-47d8-a8e2-44105126c42b)
[Screenshot Here: Azure VM IP Address]

6. IP address and location from the Azure virtual machine with the VPN connected to a ProtonVPN server in Japan.

![image](https://github.com/JasonDelahoussaye/Virtual_Private_Network_VPN_IP_Address_Observations/assets/106440235/cca59671-88f4-490d-892c-6dd93d5c5974)
[Screenshot Here: VPN IP Address]

## Understanding the Results

From this exercise, you can observe the following:

- When accessing the website from your actual PC without a VPN, it shows your original IP address and your city location.

- After connecting to the Azure virtual machine and accessing the website, a different IP address and the location of the virtual machine (e.g., Paris) are displayed.

- Finally, by connecting to the ProtonVPN server in Japan from within the virtual machine and accessing the website again, another IP address and the location of the VPN server (e.g., Tokyo, Japan) are shown.

This exercise demonstrates how VPNs work by encrypting and routing your internet traffic through remote servers, making it appear as if you are browsing from different locations. VPNs can enhance privacy, and security, and allow you to bypass geo-restrictions.
