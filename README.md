<p align="center">

<img src=https://github.com/user-attachments/assets/ff86f30e-0fb6-4f2b-81c1-c3cd90c1ff76 alt="VM logo" width="600">
</p>

<h1>Cross-Platform Virtual Machine Setup: Windows & Linux</h1>
I created this project to learn how virtualization works across different operating systems. Follow along as I build virtual machines on both Windows and Linux and break down each step.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)


<h2>Operating Systems Used </h2>

- Ubuntu
- Windows 10 Pro

<h2>Windows & Linux VM Creation: Step-by-Step Project</h2>

- Create a resource group
- Deployed a Windows VM
- Deployed a Linux VM
- Verified that both VMs were running



<h3>Step-by-Step Resource Group Setup</h3>

<p>

![1](https://github.com/user-attachments/assets/7ed7e175-cf03-47f4-9630-a46c1c941c9e)
![2](https://github.com/user-attachments/assets/8704c8ed-e944-4562-9cb6-5bd241d344c5)
</p>
<p>
1.Before we  create this VM, make a free Microsoft Azure account, and you get 200 credits for 30 days. Trust me it'll last you long as long as you dont forget to stop your Virtual Machine.
</p>
-Ok now that you have your account, we need to make a resource group. Resource groups provide organization, security, cost management, and simplified operations for Azure VMs and other resources.
</p>
2.You can click the resource group from the home screen, or you can type resource group in the search bar at the top.
</p>
3.Now here just click create.
</p>
<br />

![3](https://github.com/user-attachments/assets/fb503633-1013-4e62-bdc9-149d77242cf9)
![4](https://github.com/user-attachments/assets/18c4a8d0-5813-4fbb-8cdf-0719d0d56495)
![5](https://github.com/user-attachments/assets/8319b261-e39d-47f9-ac77-c89a3a48ed68)

</p>
-If you create a free account, you should have "Azure subscription 1" just like I do. If not, it will look different and thats okay. You can name the resource group whatever your heart desires; you can copy me if you want to. Hit next twice.
</p>
- You can now click Create
</p>
- Now that we have created our resource group, we can move on to creating a Windows VM.
<br />

<h3>Step-by-Step Windows VM setup</h3>

<p>

![6](https://github.com/user-attachments/assets/7b57014c-13f0-41e9-a44d-c2e4688f781b)
![7](https://github.com/user-attachments/assets/726337ec-b3bd-4a50-b641-4f008e0b6cab)
<p>
-Now from the resource groups page you can search up virtual machines, click on virtual machines.
</p>
-Click on create > Azure virtual machine.
<br />

<p>

![8](https://github.com/user-attachments/assets/8ecde3dc-2349-422c-9576-7cbd1d61a4fb)
![9](https://github.com/user-attachments/assets/947e190d-9345-4b8a-8f48-dccca99fa9d1)

</p>
<p>
- Here, you make sure the resource group is the same one you just made. Next, you name the Virtual machine "windows-vm".Here you make sure the Region is the same as your resource group, in this case it was (US East Us-2). For the image, make sure you select "Windows 10 Pro, version 22H2". This is a Windows VM, not a Linux.
</p>
- Now for the size, make sure you pick something that has at least 2VPUs, otherwise it will be rather slow.
</p>
- Next, create a Username and a Password, something simple that you can remember. Make sure to write this down or bring up a notepad from the Start Menu and jot that info down. Make sure you check the box under Licensing and then click Next twice until you get to Networking.
<br />

<p>

![10](https://github.com/user-attachments/assets/e6d429ac-036f-44eb-ab54-dc9df9ec5a4e)
![11](https://github.com/user-attachments/assets/d4429909-3a4d-4a24-9517-4bcf78e245bc)
</p>
<p>
-Now in Networking, we need to create a new Virtual network, click Create new, and type VM1-Vnet.
</p>
- You can now see the new name for our Virtual Network, click Review + create.
<br />

<p>

![12](https://github.com/user-attachments/assets/cbd92ebe-ed80-449b-b64a-919f9ae994dc)
![13](https://github.com/user-attachments/assets/404bffd6-02a1-4392-a9f9-0af281b643ed)
</p>
<p>
- Now if all went well, the next page should say "Validation passed." Click create.
</p>
- Finally, the next page should say "Deployment is in progress". That shouldn't take long. When it's done, it should say " Your deployment is complete". You did it! You created your first virtual machine, Now you can explore, test software, run operating systems, practice IT tasks, or safely experiment without affecting your main system.
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
