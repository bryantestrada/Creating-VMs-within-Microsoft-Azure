# Create-VMs-within-Azure
<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>Microsoft Azure- Creating Virtual Machines (Virtual Computers)</h1>
This tutorial outlines the creation of virtual computers using a cloud service provider (Microsoft Azure). Also, How to access your VM using a remote desktop on MacOS.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop

<h2>Operating Systems Used </h2>

- MacOS
- Windows 10</b> (22H2)
  
<h2>List of Prerequisites</h2>

- Microsoft Azure subscription

<h2>Objectives</h2>

- Getting Started
- Create a Resource Group
- Create a Virtual Machine
- Accessing your VM using a Remote Desktop
- Disconnect and Close your Resource Group

<h2>Getting Started</h2>
<p>
First, open portal.azure.com and sign into your account; If you don't have one, sign up for a free 30-day subscription and create a username and password (tenant). When you first sign up for Microsoft Azure, during your 30-day trial, you are given 200 credits that you can use to access paid services such as VMs, Storage accounts, etc.
<p>
<br />
  
 <img width="352" alt="Screenshot 2023-07-25 at 6 43 40 PM" src="https://github.com/bryantestrada/Deploying-AD-within-Azure-VMs/assets/133170900/897c1a9f-91eb-4cd7-941b-eb03d6539b88">
 
<br />
<h2>Create a Resource Group</h2>
<p>
Once signed in, open Resource Groups in Azure by pressing the icon or typing Resource Groups in the search bar.
</p>
<br />

<p>
<img width="512" alt="RG" src="https://github.com/bryantestrada/Deploying-AD-within-Azure-VMs/assets/133170900/0e074e67-c244-4d4e-9488-9ddd567921b6">
</p>
<p>
Then, create a Resource Group by clicking the Create button on the top left of the page.  
</p>
<br />
<img width="400" alt="RG-1" src="https://github.com/bryantestrada/Deploying-AD-within-Azure-VMs/assets/133170900/9a0b03fc-a043-4d41-b968-749e0f4e6d97">
<br />
<p>Give your Resource Group a name and a region, then click Review and Create.</p>
<img width="367" alt="RG-2" src="https://github.com/bryantestrada/Deploying-AD-within-Azure-VMs/assets/133170900/e5e90036-7f92-44af-bfeb-f9f288d380a0">
<br />
<h2>Create a Virtual Machine</h2>
<p>
Now that you have a Resource Group, Open Virtual Machines (VMs) by typing it into the search bar and create a new VM by clicking Azure  Virtual Machine in the top left of the page.
</p>
<br />
<img width="400" alt="RG-4" src="https://github.com/bryantestrada/Deploying-AD-within-Azure-VMs/assets/133170900/1bb57b73-081e-4dec-a3a8-69e8c95cade2">
<br />
<p>
When creating your Virtual Machine, store it in the Resource Group you've created, RG_1. Name your VM (VM1) and select a region (I recommend the same region as your resource group). Choose Windows 10 Pro as your operating system from the "image" dropdown menu.
</p>

<img width="400" alt="VM" src="https://github.com/bryantestrada/Deploying-AD-within-Azure-VMs/assets/133170900/90fcf1f8-d918-4498-bdcb-2064b2860def">

<br />
 <p>
  Next, scroll down and select the "size" of your VM; If you're going to be using the VM for more than just a test, I recommend selecting at least two VCPUs, because one vcpu will run slow due to the low processing capabilities. After that, input a username and password that you will use to sign into your VM from a remote desktop. Next, confirm the licensing by checking the box to accept the licensing agreements of the cloud service provider.
 </p>

 <img width="393" alt="VM2" src="https://github.com/bryantestrada/Deploying-AD-within-Azure-VMs/assets/133170900/548fb3ef-b0fb-448b-b2fb-0f357d850837">
<br />
<p>
Finally, click the Review and Create button; Azure will validate the information and give you a price estimate. This is based on how long you will need your VMs running. Click Create; Azure will deploy your Virtual Machine within your Resource group. 
</p>
<img width="400" alt="VM3" src="https://github.com/bryantestrada/Deploying-AD-within-Azure-VMs/assets/133170900/05cf139e-8c5b-47f8-8e52-e0e1b963ebbb">

<img width="512" alt="Depl" src="https://github.com/bryantestrada/Deploying-AD-within-Azure-VMs/assets/133170900/3b0b799d-0e2a-48b8-ae47-aa3e3c00096c">

<br />
<p>
It may take a while, but once the deployment is complete, you can go to the Resource Group; You should see all the resources created along with your Virtual Machine.
</p>
<img width="512" alt="RG_list" src="https://github.com/bryantestrada/Deploying-AD-within-Azure-VMs/assets/133170900/43bf4852-ecfc-4f42-a3dc-814a88e3b91f">

<br /> 
<h2>Accessing your VM using a Remote Desktop</h2>
<p>
If you don't have a Remote desktop, you can download one using the Apple store by clicking on the Apple symbol at the top left of the MacOS toolbar.
<p>
<img width="400" alt="toolbar" src="https://github.com/bryantestrada/Deploying-AD-within-Azure-VMs/assets/133170900/b1a8866d-fc29-4da7-abe6-199b9be253ed">
<p>
Type Remote Desktop in the search bar and download it for free.
</p>
<img width="512" alt="RMD" src="https://github.com/bryantestrada/Deploying-AD-within-Azure-VMs/assets/133170900/a64ac2d0-8129-4104-823e-359f9d51c6b3">
<br />
<p>
Once downloaded; Open the application and add a PC; You will need your VMs public IP address, so go back to Azure and navigate to the VM you created.
</p>
<img width="512" alt="VM_0" src="https://github.com/bryantestrada/Deploying-AD-within-Azure-VMs/assets/133170900/fdab520b-578b-4234-9739-f64640a18cc0">
<br />
<p>
Copy the public IP; It will be to connect the remote desktop to your Virtual Machine.
</p>
<img width="640" alt="Clip" src="https://github.com/bryantestrada/Deploying-AD-within-Azure-VMs/assets/133170900/2ddd782d-8a47-479c-8a20-fc79d74315e9">
<p>
Paste the IP address and click add. Once added, double-click on the new icon and input the username and password for the VM. Click Continue.
</p>
<img width="361" alt="RMD1" src="https://github.com/bryantestrada/Deploying-AD-within-Azure-VMs/assets/133170900/d23bdf84-0c8b-48c4-ac7c-8256b20eabe1">
<img width="512" alt="RMD2" src="https://github.com/bryantestrada/Deploying-AD-within-Azure-VMs/assets/133170900/c06f5fe2-9f57-4d4b-be55-053a6cec5b28">
<br />
<p>
After you've inputted the correct credentials, it may display a warning pop-up saying it's an insecure connection, disregard the message, and click continue to connect you to your VM. It may take a while to load the Virtual Machine, depending on the size you chose for your VM during its creation.
</p>
<img width="512" alt="Warning" src="https://github.com/bryantestrada/Deploying-AD-within-Azure-VMs/assets/133170900/72371920-aeed-4b88-9e7c-b035a8bc0cf3">
<br />
<p>
Accept the privacy settings, and Congratulations, you've finished setting up your Virtual Machine.
</p>
<img width="512" alt="Vm4" src="https://github.com/bryantestrada/Deploying-AD-within-Azure-VMs/assets/133170900/17f306d0-cd22-4791-8cd0-cf29ca092158">
<img width="512" alt="Vm done" src="https://github.com/bryantestrada/Deploying-AD-within-Azure-VMs/assets/133170900/0247f1c7-00bc-45ea-a07c-4134bf1e52e3">
<br />
<h2>Disconnect and Close your Resource Group</h2>
<p>
To disconnect and close your VM, click on the windows button on the bottom left corner of screen. Then click power and select disconnect. This will close the Virtual machine and you will have to sign in using your credentials the next time you log in.
</p>
<img width="512" alt="disconnecet" src="https://github.com/bryantestrada/Deploying-AD-within-Azure-VMs/assets/133170900/6cf89ce3-26cd-4f20-9f3c-184c918a4c22">
<br />
<p>
Finally, to delete the Virtual machine and all the resources created along with it; Go back to the Resource Group you created and click Delete Resource Group; you will have to type in the name of the group in the provided section and click delete.
</p>
<img width="512" alt="RG" src="https://github.com/bryantestrada/Deploying-AD-within-Azure-VMs/assets/133170900/3e0163a7-48e3-429a-bff8-438c06144493">
<img width="512" alt="Delete" src="https://github.com/bryantestrada/Deploying-AD-within-Azure-VMs/assets/133170900/729da1f1-3d5f-461a-b73e-fe001207678b">
<br />
<p>
And thats it! You should now know how to create, access, and delete Virtual Machines within Microsoft Azure using MacOS.
</p>
