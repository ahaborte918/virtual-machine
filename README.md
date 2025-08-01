<p align="center">

<img src=https://github.com/user-attachments/assets/ff86f30e-0fb6-4f2b-81c1-c3cd90c1ff76 alt="VM logo" width="600">
</p>

<h1>Cross-Platform Virtual Machine Setup: Windows & Linux</h1>
In this project we will demonstrate the setup and configuration of Virtual Machines running both Windows and Linux operating systems (OS). It explores virtualization concepts while showcasing cross-platform environment creation for development and network testing.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)


<h2>Operating Systems Used </h2>

- Ubuntu
- Windows 11 (24H2)

<h2>STEPS INCLUDED</h2>

- STEP 1 - Create a Resource Group
- STEP 2 - Create a virtual machine for Windows
- STEP 3 - Deploy the Windows VM
- STEP 4 - Create a virtual machine for Linux
- STEP 5 - Deploy the Linux VM
- STEP 6 - Verify that both VMs are running



<h2>Step-by-Step Resource Group Setup</h2>

<p>
The very first thing we have to do is sign-up for a free Microsoft Azure account. When your account is created you are awarded a $200 credit that expires in 30 days. 
After an account has been made we can began our project by creating a Resource Group. Resource Groups provide organization, security, cost management, and simplified operations for Azure VMs and other resources.
</p>
You can click on the Resource Group from the home screen or you can type Resource Group in the search bar at the top. Click on Create and let's get started.
</p>

<img width="785" height="413" alt="Resource Group SS1" src="https://github.com/user-attachments/assets/2d54b42e-bb27-4ae6-8d29-cfe8a714dbe3" />
<img width="809" height="395" alt="Resource Group SS2" src="https://github.com/user-attachments/assets/943c5f69-2c12-4331-af47-71643f92e697" />

</p>
<p>

</p>
You can click on the Resource Group from the home screen or you can type Resource Group in the search bar at the top. Click on Create and let's get started.
</p>
<br />

<img width="1397" height="692" alt="Windows VM 1" src="https://github.com/user-attachments/assets/f7909e80-80f6-446e-b4d9-3f1043e982ae" />


</p>
-If you create a free account, you should have "Azure subscription 1" just like I do. If not, it will look different and thats okay. You can name the resource group whatever your heart desires; you can copy me if you want to. Hit next twice.
</p>
- You can now click Create
</p>
- Now that we have created our resource group, we can move on to creating a Windows VM.
<br />

<h3>Step-by-Step Windows VM setup</h3>

<p>

<img width="1525" height="685" alt="Windows VM 2" src="https://github.com/user-attachments/assets/cf944d3c-6dfb-429b-85db-9241e0d84886" />


<p>
- Click Home tab and you be bough to the main page. From there type virtual machines in the search bar.
</p>
-Click on create > virtual machine.
<br />

<p>

<img width="1233" height="699" alt="Windows VM 3" src="https://github.com/user-attachments/assets/6af67b23-0191-47c7-9184-a926bd052e86" />
<img width="1399" height="746" alt="Windows VM 4" src="https://github.com/user-attachments/assets/92edf88f-cf6a-4e15-b72f-b316130c40b2" />

<p>
- Here, we want to ensure the Resource Group is the same one we just created "VM-Project". Next, you will give the Virtual Machine a name:"WindowsVM". Make sure that the same Region is picked, reminder - we selected (US East Us-2) as our Region when we created the Resource Group previously. For the line that says "Image" scroll down and select "Windows 11 Pro, version 22H2 (or Windows 10 Pro, version 22H2 if you do not have W11)". This is going to be our Windows virtual machine.
</p>
- Now for the size, make sure you pick something that has at least 2VPUs, otherwise it will be rather slow.
</p>
- Next, create a Username and a Password, something simple that you can remember. Make sure to write this down or bring up a notepad from the Start Menu and jot that info down. Make sure to check the box under 'Licensing' at the bottom and then click Next to skip over Disk section so you can get to to Networking.
<br />

<p>

<img width="1139" height="773" alt="Windows VM 5" src="https://github.com/user-attachments/assets/c71990bf-7558-4f43-a50a-223526ebe0ec" />


</p>
<p>
-Now in Networking, we need to create a new Virtual network, click Create new, and type WindowsVM1-Vnet.
</p>
- You can now see the new name for our Virtual Network so we are ready to click Review + create at the very bottom.
<br />

<p>

<img width="1342" height="746" alt="Windows VM 6" src="https://github.com/user-attachments/assets/09d4cec5-d1bf-4420-85ff-afd39e753bbc" />

</p>
<p>
- If all went well, the next page should say "Validation passed." Once you see it go ahead and click on Create.
  
</p>

<img width="1466" height="705" alt="Windows VM 8" src="https://github.com/user-attachments/assets/5f90b873-793d-482a-9a54-e9ae368fe790" />


- The next page should say "Deployment is in progress" and start loading, followed immediately by "Your deployment is complete" once the loading is complete. Guess what!! You just set up your first virtual machine! Congrats because now you'll be able to explore, test software, run operating systems, practice IT tasks, even safely experiment without affecting your main system!
<br />
<h2>How to create a Linux VM</h2>
<p>

![14](https://github.com/user-attachments/assets/4f859956-aa8c-4ab2-9635-8b886f23cfec)
</p>
<p>
-Now, under Virtual machines, you see we created the Windows-VM. We create our Linux VM, click Create> Azure Virtual Machine.
</p>
<br />

<p>

![15](https://github.com/user-attachments/assets/07025c52-4351-411c-9f15-84d6554b5c36)
</p>
<p>
Here we keep the same Resource group, for the Virtual machine, name it "linux-vm". Same Region. Now, for the image, choose  "Ubuntu Server 22.02", which is for Linux VM.
</p>
<br />

<p>
</p>

![16](https://github.com/user-attachments/assets/75f289bc-0fe2-4423-b06d-10c97713a5a2)
<p>
-Scroll down and make sure we have at least 2 vCPUs again. For the Authentication type, choose Password.
</p>
- You can use the same info as we did in the Windows VM, or choose your own.
</p>
- Then click next twice until you get to Networking. 
<br />

<p>

![17](https://github.com/user-attachments/assets/6e254f72-865c-4711-8374-4ca4cf7590fd)
</p>
<p>
- Next, we will keep the same virtual network as the Windows VM. In this case, it was "VM1-Vnet". Now, click Review + create.
</p>
<br />

<p>
  
![18](https://github.com/user-attachments/assets/99b74b49-4dbe-4883-ac7c-3478e6cade9b)
</p>
<p>
- The screen should look like this, which means you created your Linux VM. You did it again! We have now created both our Windows and Linux VM.
</p>
<br />

<p>

![19](https://github.com/user-attachments/assets/916186f1-51b5-4552-9f8a-050d94b9cd57)
</p>
<p>
-Lastly, I would like to move you back to our Virtual machines. Here, we confirm that our Linux and Windows VMs have been successfully created and are running. If you are done with this lab, you can click the box next to Names and then hit delete on the top right.
</p>
<br />

<h2>Final Thoughts</h2>
</p>
- I just finished setting up both a Windows and a Linux virtual machine, and honestly, it was a great learning experience. It helped me get more comfortable with the installation process, managing system resources, and understanding how different operating systems work. I also got a better feel for how virtualization plays a big role in IT and troubleshooting.<br />
