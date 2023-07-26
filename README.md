# Create-VMs-within-Azure
<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>Microsoft Azure- Creating Virtual Machines (Virtual Computers)</h1>
This tutorial outlines the creation of virtual computers using a cloud service provider (Microsoft Azure).<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop

<h2>Operating Systems Used </h2>

- Windows 10</b> (22H2)
  
<h2>List of Prerequisites</h2>

- Microsoft Azure subscription

<h2>Objectives</h2>

- Sign in
- Create a Resource Group
- Create a Virtual Machine

<h2>Sign in</h2>
<p>
First, open up portal.azure.com and sign into your account, if you dont have one you can sign up for a free 30 day subscription and create a username and password (tenant).
<p>
<br />
  
 <img width="352" alt="Screenshot 2023-07-25 at 6 43 40 PM" src="https://github.com/bryantestrada/Deploying-AD-within-Azure-VMs/assets/133170900/897c1a9f-91eb-4cd7-941b-eb03d6539b88">
 
<br />
<h2>Create a Resource Group</h2>
<p>
Once you're signed in, open up Resource Groups in Azure by pressing on the icon or by typing Resource Groups in the search bar.
</p>
<br />

<p>
<img width="512" alt="RG" src="https://github.com/bryantestrada/Deploying-AD-within-Azure-VMs/assets/133170900/0e074e67-c244-4d4e-9488-9ddd567921b6">
</p>
<p>
Then, create a Resource Group by clicking on the create button on the top left of the page.  
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
To create the VM, first store the VM within the Reource Group you've created by selecting it in the dropdown menu (RG_1).
Then, give your VM a name (VM1) and select a region (I recommend the region you used for the resource group).
Next, choose Windows 10 pro as your operating system (OS) by selecting it in the "image" dropdown menu.
</p>

<img width="400" alt="VM" src="https://github.com/bryantestrada/Deploying-AD-within-Azure-VMs/assets/133170900/90fcf1f8-d918-4498-bdcb-2064b2860def">

