# CREATING A VIRTUAL MACHINE IN THE HYPER-V MANAGER
In this project will show the step by step process how a virtual machine can be created in the Hyper-V Manager.

To start the process of creating the virtual machine you will first download the **iso** image of the virtual machine and save in any folder or path that it can be recalled at anytime.

Step1 - By default you do not have the Hyper-V Manager on the system, in other to confirm if its active on your system press the Windows key and search for Hyper-V Manager in your application otherwise press **Windows + R** and hit **Enter** on your key board to check/select the option, click ok and restart the system for the settings to initialize.

![Alt text](<Images/Windows plus R.png>)
![Alt text](<Images/Check the Hyper-V option.png>)

Step2 - Search and open the Hyper-V Manager on your machine and follow the below step:
* Select Action
* Connect to Server
* Select Local computer
![Alt text](<Images/Check the Hyper-V option.png>)

Step3 - Create a virtual switch manager, for the project will choose the option of private switch as it allows communication between virtual machines on the same private network no internet connectivity, external network or connection to the host operating machine. Follw the steps below to create the virtual switch manager.
* On the Hyper-V Manager, select Action
* Select virtual swtich manager.
* Select New virtual network. 
* Select External.
* Select create virtual switch.
* Give a name of your choice to the Virtual Manager.
* On connection type choose Private network.
* Select Apply and Ok for the settings to initialize.

![Alt text](<Images/Choose External.png>)
![Alt text](<Images/rename choose private network and click apply.png>)

At this point we have successfully created the switch next we need to create the virtual machine, but remember this is where we use the **iso image** that was downloaded, kindly follow the below steps to inatll the virtal machine.

## Step 1
* On the Hyper-V Manager, select Action at the top bar left or New at the right.
* Select virtual machine to diaplay the Virtual machine wizard.
* Read the message on the Before you begin to choose what best for you.
* For this project will Click on next. 

![Alt text](<Images/creating a virtual machine action new new vM.png>)

## Step 2 
* The next page allows you to either choose a storage location or you can create a new folder and select the created folder as your storage location, ensure to tick the box if you change the default storage path.
![Alt text](<Images/Changed storage location to cVM.png>)

## Step 3
Select a Generation, we see two generations (1 and 2)
**N/B** Your choice to create a generation 1 or generation 2 virtual machine depends on which guest operating system you want to install and the boot method you want to use to deploy the virtual machine. We recommend that you create a generation 2 virtual machine to take advantage of features like Secure Boot.

Generation 1 virtual machines support most guest operating systems. 
Generation 2 virtual machines support most 64-bit versions of Windows and more current versions of Linux and FreeBSD operating systems. For more information kindly click [here](https://learn.microsoft.com/en-us/windows-server/virtualization/hyper-v/plan/should-i-create-a-generation-1-or-2-virtual-machine-in-hyper-v)

For this project I will choose generation 2 as this suits what I want to achive.
![Alt text](<Images/Choosed generation 2.png>)

## Step 4
* Allow the selected option of Dynamic memory as this feature allows you to dynamically allocate memory resources to the VMs running in Hyper-V environments. This functionality reclaims a part of unused memory from VMs that don’t need it at that particular moment and then reassigns the reclaimed memory to other VMs that actually require it. However here the size depends on the system RAM.
![Alt text](<Images/memory assigned and choosed dynamic momory.png>)

## Step 5
* On the network configuration I choosed the name of the virtual switch I configured early, which is a private network.
![Alt text](<Images/the previous network created at the first step.png>)

## Step 6 - Configure Networking
* The vritual machine requires storage space to install the operating system, its just like a hard disk on your system but this will be a storage space virtually. Also note that the path will be same as the location initially specified.
![Alt text](<Images/virtual hard disk 40gb.png>)

## Step 7 - Installation Options
* This is the installation option where you choose the **ISO image** you already downloaded.
![Alt text](<Images/choosed the location of my iso image downloaded.png>)

## Step 8 - Summary 
* This page shows you the summary of settings/configuration made while setting up the Virtual machine.
![Alt text](<Images/Summary of the installation.png>)


