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
2.) Now head to the virtual machine icon, or simply type in the search bar "Virtual Machines".



![image](https://i.imgur.com/bVQrMdu.png)



2.) Now head to the virtual machine icon, or simply type in the search bar "Virtual Machines".
3.) You should now see the homepage of the Virtual Machine tab.



![image](https://i.imgur.com/NpJNDW8.png)



3.) You should now see the homepage of the Virtual Machine tab.
4.) Click on the top left dropdown where it says Create, and choose Azure Virtual Machine.



![image](https://i.imgur.com/49ZyZJ3.png)



4.) Click on the top left dropdown where it says "Create" and choose Azure Virtual Machine.
5.) Now you're in the process of choosing your Virtual Machine specs.



![image](https://i.imgur.com/hePU6LU.png)



5.) Now you're in the process of choosing your Virtual Machine specs.
6.) Start off by making sure you have a current subscription, and we're going to name this Virtual Machine "VM1" (also take notice that we didn't have a resource group created, but it automatically populates one for you.) Set the region to wherever you want this machine to be. For the experiment I'll select Sweden Central. Than we're going to choose Windows 10 for the image.



![image](https://i.imgur.com/3qQm04x.png)

  

6.) We're going to name this Virtual Machine "VM1" (also take notice that we didn't have a resource group created, but it automatically populates one for you.) Set the region to wherever you want this machine to be. For this tutorial, I'll select Japan East (You will see how this affects your virtual machine later). Then we're going to choose Windows 10 for the image.

7.) Now choose the size, we'll use "2 VCPUS,16 GIB Memory", and our username will be "labuser" and the password will be "Password1VM1". Make sure you click the windows checkbox, and than hit review and create!
  


![image](https://i.imgur.com/uqpFYhu.png)



7.) For the size, we'll use "2 VCPUS,16 GIB Memory". Our username will be "labuser" and the password will be "Password1VM1". Make sure you click the Windows checkbox, and then hit review and create.
8.) You should get a validation passed, and than hit create.



![image](https://i.imgur.com/QFYiD4F.png)



8.) You should get a validation passed, then hit create.
9.) Allow the Virtual Machine to deploy, ths may take a few minutes,
  
 

![image](https://i.imgur.com/CFmqrGE.png)

 

9.) Allow the Virtual Machine to deploy (This may take a few minutes).
10.) The deployment should now be complete.



![image](https://i.imgur.com/8HAcMDr.png)



10.) The deployment should now be complete.
11.) Click go to resource, it'll take you straight to the VM.



![image](https://i.imgur.com/0pB1qtc.png)



11.) Click, "Go to resource".
12.) You may see a lot of things going on, but for now just focus on the public IP address, that's what we want. So copy that.
  


![image](https://i.imgur.com/M7DHJUB.png)



12.) You may see a lot of things going on, but for now, just focus on the public IP address and copy it. 
13.) Now press the windows key either on your keyboard or on the screen. Type "RDC" and you should see "Remote Desktop Connection" click that.



![image](https://i.imgur.com/lJCrb00.png)



13.) I am using a Mac so I will be using the Microsoft Remote Desktop app. Open the application and select "Add PC".
14.) You should see the login pop-up, now paste that IP address into the pop-up, and hit connect.
  


![image](https://i.imgur.com/ZYWrqpx.png)



14.) You should see a pop-up to input an IP address. Paste the IP address into the pop-up, and hit "Add".
15.) You'll now be prompted to log in with a username and password. Using the one we created in the beginning log in, (labuser1 - username, Password1VM1 - passsword) you should see a prompt saying "Do you want to connect anyways?" Click yes.
  


![image](https://i.imgur.com/qaoGD9r.png)



15.) You'll be prompted to log in with a username and password. Using the ones we created, in the beginning (labuser - username, Password1VM1 - password), hit continue to login. 
16.) You should be taken inside the Virtual Machine, if you used the labuser name, it should log you into the Virtual Machine as "labuser", you'll then see a prompt asking you to check and uncheck some things, for this experiment uncheck all and hit accept.

  

![image](https://i.imgur.com/SwdqUty.png)



16.) You should be taken inside the Virtual Machine, if you used the labuser name, it should log you into the Virtual Machine as "labuser", you'll then see a prompt asking you to check and uncheck some things, for this experiment uncheck all and hit accept.
17.) You're now inside a virtual machine! Now remember I selected Sweden as my Virtual Machine location. What do you think my Google would look like? Boom! Because I set my Virtual Machine location to Sweden it acts as a computer connected to a network in Sweden! Pretty cool right?



![image](https://i.imgur.com/PmjJwF1.png)



17.) You're now inside a virtual machine! Now remember I selected Japan as my Virtual Machine location. What do you think my Google would look like?
18.) Boom! Because I set my Virtual Machine location to Japan it acts as a computer connected to a network in Japan! Pretty cool right? 
19.) Now after you're done with your Virtual Machine let's head back to clean up our project. So hit the windows key or click the icon on your computer and type CMD to open command prompt, type "logoff"



19.) Now after you're done with your Virtual Machine let's head back to clean up our project. So hit the windows key or click the icon on your computer and type CMD to open command prompt, type "logoff"
20.) Now you should be back inside the Azure Portal, and looking inside the Virtual Machine specs and settings. Now click delete.



![image](https://i.imgur.com/ESWex7r.png)



18.) Boom! Because I set my Virtual Machine location to Japan it acts as a computer connected to a network in Japan! Pretty cool right? 
19.) Now after you're done with your Virtual Machine let's head back to clean up our project. So hit the windows key or click the icon on your computer and type CMD to open command prompt, type "logoff"
20.) Now you should be back inside the Azure Portal, and looking inside the Virtual Machine specs and settings. Now click delete.



![image](https://i.imgur.com/mSvgDeb.png)



19.) Now after you're done with your Virtual Machine make sure you log out of the virtual machine. Once that is done you should be back in the Azure portal, and looking inside the Virtual Machine settings. Find and click the "Delete" button. 
21.) You'll now see the option to delete, you want to click all the boxes, to delete the Network Interface and Public IP address. Click delete. Give it a minute or two to delete.


![image](https://i.imgur.com/qjT77O9.png)



20.) You'll now see the option to delete, you want to click all the boxes, to delete the Network Interface and Public IP address. Click delete. Give it a minute or two to delete.
21.) Boom. Should be done now. Going back to the Home for the Virtual Machines, it should be cleared out.



![image](https://i.imgur.com/M2xc017.png)



21.) Boom! It should be done now. Go back to the home page for the Virtual Machines, it should be cleared out.
22.) Now you're not quite done yet. Click the search bar and type "Resource Groups", you should now be looking at your current resource groups.



![image](https://i.imgur.com/XuOHq1c.png)



22.) Now you're not quite done yet. Click the search bar and type "Resource Groups". You should see your current active resource groups.



![image](https://i.imgur.com/km5vweT.png)



24.) Click the Resource Group that was automatically created when we created our Virtual Machine and click "Delete Resource Group".
25.) Now type the name of the resource group, and click delete.



![image](https://i.imgur.com/B42lKhM.png)



25.) Now type the name of the resource group, and click delete. Do the same for any other resource groups that need to be deleted.



![image](https://i.imgur.com/yaKQ26C.png)



25.) CONGRATS!! You have now created your first Virtual Machine!
