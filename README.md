<p align="center">
<img src="https://i.imgur.com/LjLZShf.jpeg" alt="Microsoft Active Directory Logo"/>
</p>


<h1>Setup and Deployment of VMs (Azure)</h1>
This tutorial outlines the setup and deployment of Azure virtual machines using Remote Desktop Protocol (RDP).<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How to Deploy on-premises Active Directory within Azure Compute](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Google Chrome
- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Step 1: Create an account on Microsoft Azure
- Step 2: Create a resource group
- Step 3: Create a virtual machine (VM) and place it into the previously created resource group
- Step 4: Take the VM's public IP address, and access the VM through Remote Desktop Connection

<h2>Deployment and Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/70co5im.jpeg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
First, you'll need to create an account on Microsoft Azure. Select whatever plan fits your needs best, but for this tutorial, the free plan has been chosen. From the main page shown above, type into the search box, "resource groups", and select the pop-up. 
</p>
<br />

<p>
<img src="https://i.imgur.com/lm419bR.jpeg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Next, select "+ Create" and enter the name for the resource group. The name does not matter, as long as you can remember it for future steps. The name for this example is "RG-VM-Example." Then, set your region to whatever area of the world you live in, and select "review + create." Make sure everything looks correct before selecting "create" once more. Wait for the resource group to be deployed, and then enter "virtual machines" into the search box. 
</p>
<br />

<p>
<img src="https://imgur.com/28fdc0cd-298c-4637-8c92-369f323186aa" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<p>
<img src="https://i.imgur.com/REJuq6Z.jpeg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Again, select "+ create", and then "virtual machine". Next, place this virtual machine into the resource group previously created. There are a multitude of different options for VM creation, but this example will be creating a Windows 10 Pro VM image. Choose the options that best fit your needs, such as region (place the VM in the same region as the RG), the size, and a username/password you can remember. Then, make sure to scroll all the way down and select the licensing box at the bottom. With the creation of this VM, Azure is going to also create a brand new subnet. Any additional VMs that you create should be placed on the same subnet, which you can find on the "Networking" tab in VM creation. But since this is the first VM, do not worry about this step. Finally, create the VM and wait for deployment. 
</p>
<br />
