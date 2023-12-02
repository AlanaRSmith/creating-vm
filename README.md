# creating-vm
![image](https://github.com/AlanaRSmith/creating-vm/assets/152671380/b34ccd0c-19b6-45a1-80bf-89643bd1be3b)

Creating a VM in Azure!
This tutorial outlines the process of creating a VM using Microsoft Azure.

1.) The first thing you are going to want to do is create a virtual machine by going to https://portal.azure.com/. First login to azure. You should see the home screen, that looks like this image below.

![image](https://github.com/AlanaRSmith/creating-vm/assets/152671380/2d95279a-1bd0-4635-a287-eff703802fdc)


2.) Now head to the virtual machine icon, or simply type in the search bar "Virtual Machines".

![image](https://github.com/AlanaRSmith/creating-vm/assets/152671380/007d8bb9-f997-446b-a259-f35dd03758f8)



3.) You should now see the homepage of the Virtual Machine tab.

![image](https://github.com/AlanaRSmith/creating-vm/assets/152671380/95002365-f1ba-4cd4-a77f-b3d9a8b1572d)


4.) Click on the top left dropdown where it says Create, and choose Azure Virtual Machine.

![image](https://github.com/AlanaRSmith/creating-vm/assets/152671380/526d076f-8885-4424-9798-28c801fe937d)


5.) Now you're in the process of choosing your Virtual Machine specs.

![image](https://github.com/AlanaRSmith/creating-vm/assets/152671380/10385d5f-770a-40f0-a931-dbd954f9c61e)


6.) Start off by making sure you have a current subscription, and we're going to name this Virtual Machine "VM-1" (also take notice that we didn't have a resource group created, but it automatically populates one for you.) Set the region to wherever you want this machine to be. For the experiment I'll select Sweden Central. Than we're going to choose Windows 10 for the image.

![image](https://github.com/AlanaRSmith/creating-vm/assets/152671380/5ada0364-8d4d-4afb-9f89-df2ad614dd57)


7.) Now choose the size, we'll use "2 VCPUS,16 GIB Memory", and our username will be "labuser1" and the password will be "Password1VM1" make sure you click the windows checkbox, and than hit review and create!

![image](https://github.com/AlanaRSmith/creating-vm/assets/152671380/59c5ba3b-be6c-4206-a78d-54164327ce83)


8.) You should get a validation passed, and than hit create.

![image](https://github.com/AlanaRSmith/creating-vm/assets/152671380/1b23c2e3-6f7c-4b5a-b8e1-1d66536813bc)


9.) Allow the Virtual Machine to deploy, ths may take a few minutes,

![image](https://github.com/AlanaRSmith/creating-vm/assets/152671380/a869228e-6a2f-4298-82dc-6ad55fc9a5d0)


10.) The deployment should now be complete.

![image](https://github.com/AlanaRSmith/creating-vm/assets/152671380/62d68197-1145-462a-99d4-e3edcdb4c63c)


11.) Click go to resource, it'll take you straight to the VM.

![image](https://github.com/AlanaRSmith/creating-vm/assets/152671380/a9ae6d80-8d90-4338-9a9e-73d8751dfd37)


12.) You may see a lot of things going on, but for now just focus on the public IP address, that's what we want. So copy that.

![image](https://github.com/AlanaRSmith/creating-vm/assets/152671380/cda508af-cb2a-4132-8c53-1e45d102051d)


13.) Now press the windows key either on your keyboard or on the screen. Type "RDC" and you should see "Remote Desktop Connection" click that.

![image](https://github.com/AlanaRSmith/creating-vm/assets/152671380/39b2823c-3dff-40c5-9216-9746507b8e88)


14.) You should see the login pop-up, now paste that IP address into the pop-up, and hit connect.

![image](https://github.com/AlanaRSmith/creating-vm/assets/152671380/8100ad78-d893-448d-935c-e40a9ade4eec)


15.) You'll now be prompted to log in with a username and password. Using the one we created in the beginning log in, (labuser1 - username, Password1VM1 - passsword) you should see a prompt saying "Do you want to connect anyways?" Click yes.

![image](https://github.com/AlanaRSmith/creating-vm/assets/152671380/f66c4c2d-f4fb-49c4-b6c6-4fc17a0ce0e6)


16.) You should be taken inside the Virtual Machine, if you used the labuser1 name, it should log you in to the Virtual Machine as "labuser1", you'll than see a prompt asking you to check and uncheck some things, for this experiment uncheck all and hit accept.

![image](https://github.com/AlanaRSmith/creating-vm/assets/152671380/6357a5a1-2a7a-41d3-908b-df34007aab8a)


17.) You're now inside a virtual machine! Now remember I selected Sweden as my Virtual Machine location. What do you think my Google would look like? Boom! Because I set my Virtual Machine location to Sweden it acts as a computer connected to a network in Sweden! Pretty cool right?

![image](https://github.com/AlanaRSmith/creating-vm/assets/152671380/f7695b56-483f-4224-a482-c29de0cde976)


18.) Now after you're done with your Virtual Machine let's head back to clean up our project. So hit the windows key or click the icon on your computer and type CMD to open command prompt, type "logoff"

19.) Now you should be back inside the Azure Portal, and looking inside the Virtual Machine specs and settings. Now click delete.

![image](https://github.com/AlanaRSmith/creating-vm/assets/152671380/5df58dc8-8461-4e5e-8e08-da683c283681)


20.) You'll now see the option to delete, you want to click all the boxes, to delete the Network Interface and Public IP address. Click delete. Give it a minute or two to delete.

![image](https://github.com/AlanaRSmith/creating-vm/assets/152671380/ae88391e-accd-451f-b411-b4d870ee93db)


21.) Boom. Should be done now. Going back to the Home for the Virtual Machines, it should be cleared out.

![image](https://github.com/AlanaRSmith/creating-vm/assets/152671380/71644009-0edf-432d-b8fc-32a39a43afdf)



22.) Now you're not quite done yet. Click the search bar and type "Resource Groups", you should now be looking at your current resource groups.

![image](https://github.com/AlanaRSmith/creating-vm/assets/152671380/41a280ee-36d2-493c-b00b-62b99d9ba8f0)


23.) Now click that Resource Group whcih was automatically created when we created our Virtual Machine. And now click "Delete Resource Group".

![image](https://github.com/AlanaRSmith/creating-vm/assets/152671380/29b531e0-adc8-4052-8d8b-b5857668f99d)


24.) Now type the name of the resource group, and click delete.

![image](https://github.com/AlanaRSmith/creating-vm/assets/152671380/25c36473-2ee3-4703-8d58-aea54bd52518)


25.) CONGRATS!! You have now created your first Virtual Machine! 
