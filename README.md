![image](https://i.imgur.com/HLsTXdH.png)



<h1>Creating a VM in Azure!</h1>
This tutorial outlines the process of creating a VM using Microsoft Azure on a Mac.<br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Computer)
- Remote Desktop
<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Azure Virtual Machine
- Link to the Azure Portal: https://portal.azure.com
- Microsoft Remote Desktop

<h2>Steps</h2>



![image](https://i.imgur.com/BqUa64Y.png)



1.) The first thing you will do is visit the website, https://portal.azure.com. Login to your account or create one once you get to the website. After logging in or creating your account, you should see the home screen that looks like the image above.



![image](https://i.imgur.com/bVQrMdu.png)



2.) Now head to the virtual machine icon, or simply type in the search bar "Virtual Machines".


![image](https://i.imgur.com/NpJNDW8.png)



3.) You should now see the homepage of the Virtual Machine tab.



![image](https://i.imgur.com/49ZyZJ3.png)



4.) Click on the top left dropdown where it says "Create" and choose Azure Virtual Machine.



![image](https://i.imgur.com/hePU6LU.png)



5.) Now you're in the process of choosing your Virtual Machine specs.



![image](https://i.imgur.com/3qQm04x.png)

  

6.) We're going to name this Virtual Machine "VM1" (also take notice that we didn't have a resource group created, but it automatically populates one for you.) Set the region to wherever you want this machine to be. For this tutorial, I'll select Japan East (You will see how this affects your virtual machine later).
  


![image](https://i.imgur.com/uqpFYhu.png)



7.) We will choose "Windows 10" for the image and "2 VCPUS,16 GIB Memory" for the size. Our username will be "labuser" and the password will be "Password1VM1". Make sure you click the Windows checkbox, and then hit review and create.
  
 

![image](https://i.imgur.com/CFmqrGE.png)

 

8.) You should get a validation passed, then hit create.



![image](https://i.imgur.com/8HAcMDr.png)



9.) Allow the Virtual Machine to deploy (This may take a few minutes).



![image](https://i.imgur.com/0pB1qtc.png)



10.) The deployment should now be complete. Click, "Go to resource".
  


![image](https://i.imgur.com/M7DHJUB.png)



11.) You may see a lot of things going on, but for now, just focus on the public IP address and copy it. 



![image](https://i.imgur.com/lJCrb00.png)



12.) I am using a Mac so I will be using the Microsoft Remote Desktop app. Open the application and select "Add PC".
  


![image](https://i.imgur.com/ZYWrqpx.png)



13.) You should see a pop-up to input an IP address. Paste the IP address into the pop-up, and hit "Add".



![image](https://i.imgur.com/qaoGD9r.png)



14.) You'll be prompted to log in with a username and password. Using the ones we created, in the beginning (labuser - username, Password1VM1 - password), hit continue to login. 

  

![image](https://i.imgur.com/SwdqUty.png)



15.) You should be taken inside the Virtual Machine, if you used the labuser name, it should log you into the Virtual Machine as "labuser", you'll then see a prompt asking you to check and uncheck some things, for this experiment uncheck all and hit accept.



![image](https://i.imgur.com/PmjJwF1.png)



16.) You're now inside a virtual machine! Now remember I selected Japan as my Virtual Machine location. What do you think my Google would look like?



![image](https://i.imgur.com/ESWex7r.png)



17.) Boom! Because I set my Virtual Machine location to Japan it acts as a computer connected to a network in Japan! Pretty cool right? 



![image](https://i.imgur.com/mSvgDeb.png)



18.) Now after you're done with your Virtual Machine make sure you log out of the virtual machine. Once that is done you should be back in the Azure portal, and looking inside the Virtual Machine settings. Find and click the "Delete" button. 



![image](https://i.imgur.com/qjT77O9.png)



19.) You'll now see the option to delete, you want to click all the boxes, to delete the Network Interface and Public IP address. Click delete. Give it a minute or two to delete.



![image](https://i.imgur.com/M2xc017.png)



20.) Boom! It should be done now. Go back to the home page for the Virtual Machines, it should be cleared out.



![image](https://i.imgur.com/XuOHq1c.png)



21.) Now you're not quite done yet. Click the search bar and type "Resource Groups". You should see your current active resource groups.



![image](https://i.imgur.com/km5vweT.png)



22.) Click the Resource Group that was automatically created when we created our Virtual Machine and click "Delete Resource Group".



![image](https://i.imgur.com/B42lKhM.png)



23.) Now type the name of the resource group, and click delete. Do the same for any other resource groups that need to be deleted.



![image](https://i.imgur.com/yaKQ26C.png)



24.) CONGRATS!! You have now created and cleaned up your first Virtual Machine!
