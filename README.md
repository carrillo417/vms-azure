
<p align="center">
  
 <img src="https://i.imgur.com/vlSVP3D.png" height="25%" width="25%" alt="Microsoft Azure Logo"/>

</p>

<h1>Creating Virtual Machines in Azure</h1>
This tutorial outlines how to create a Windows 10 Virtual Machine as well as a Linux Ubuntu Virtual Machine in Azure.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)


<h2>Operating Systems Used </h2>

- Linux Ubuntu
- Windows 10 Pro (22H2)

<h2> Creating a Windows Virtual Machine </h2>


  - Go to portal.azure.com 
  - Create a resource group, you can either click on the resource groups on the homepage or use the search feature as shown below.
  <br />
  <img src="https://i.imgur.com/0tGFyCZ.png" height="80%" width="80%" alt=""/>

  <br />

<img src="https://i.imgur.com/NiL5dOJ.png" height="80%" width="80%" alt=""/>

- Click on Create and name your resource group (Remember the region selected as this is important for later on)
<img src="https://i.imgur.com/DNw9Fkd.png" height="80%" width="80%" alt=""/> 
<br />
<img src="https://i.imgur.com/IoYcFgV.png" height="80%" width="80%" alt=""/>

- Now we are ready to create our Windows virtual machine, search for virtual machines and create a Windows VM
  
<img src="https://i.imgur.com/SuTMrP6.png" height="80%" width="80%" alt=""/>

- Select Azure virtual machine
<img src="https://i.imgur.com/Yy6UcZa.png" height="80%" width="80%" alt=""/>

- Select the resource group we created
- name your VM
- Select the same region as your resource group
- For image select Windows 10 Pro version 22H2
- For size make sure you select anything with 2 vcpus or more (2 vcpus should be enough for the activities we will be doing)
<img src="https://i.imgur.com/xKMnQVo.png" height="80%" width="80%" alt=""/>

- Create an username and password (make sure you remember it as this is how we are going to access the VM)
- Make sure to check the Licensing box, otherwise you won't be able to create the VM
<img src="https://i.imgur.com/UiQ7pO2.png" height="80%" width="80%" alt=""/>

- The Networking tab is where the Virtual network is created, if you select 'Create new' you are able to rename it. We will be using this vnet for our Linux VM as well.

<img src="https://i.imgur.com/taKnb7J.png" height="80%" width="80%" alt=""/>

- Create the Windows virtual machine 
<img src="https://i.imgur.com/SgUics4.png" height="80%" width="80%" alt=""/>

<h2> Creating a Linux Virtual Machine </h2> 

- Create a new virtual machine
- Select the same resource group as the Windows VM
- Name the VM and select the same region as the Windows VM
- For image select Ubuntu Server 22.04 or Ubuntu Server 24.04
- The size should be at least 2 vcpus 

<img src="https://i.imgur.com/V9N07dh.png" height="80%" width="80%" alt=""/> 

- For the authentication type select Password, create Username and Password and remember as this is how we access the Linux VM

<img src="https://i.imgur.com/dvUMlRs.png" height="80%" width="80%" alt=""/> 

- Under Networking, make sure the virtual network is the same as the Windows VM, now we are able to create our Linux VM

<img src="https://i.imgur.com/kV88V9Q.png" height="80%" width="80%" alt=""/> 

We have succesfully created a Windows and Linux VM. We are able to see them in our Resource Group we created earlier. 

<img src="https://i.imgur.com/RZTfSE8.png" height="80%" width="80%" alt=""/>

                                      
