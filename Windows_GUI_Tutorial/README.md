# Windows GUI Tutorial

This tutorial will take you through the process of setting up a Google Compute Engine VM in the form of a Windows Server with a GUI. We will be utilizing [the Google Compute Engine Service](https://cloud.google.com/compute) to set up a VM. Additionally, this tutorial will go through setting up a Python development environment with Anaconda and Visual Studio Code.  

- Create a Google Cloud Platform (GCP) account and then click this [link](https://cloud.google.com/compute) to jump to the service. 
- Find the "Go to Console" button and click it. It wil bring you to your VM instances page assuming you are signed into your GCP account.
- From the top panel of the instances page, click the "Create Instance" button. This will bring you to the VM creation page. 
- Give your VM instance a name and set your region to your desired server location. In this example, I have chosen Montreal. I have also chosen a general purpose machine for this example and machine with lower specificiations. In a real use case, these specifications will change as you will need more resources to perform heavy processing

![](https://github.com/Samir-Sell/Cloud_Computing_Google/blob/main/Images/mtyp.png)

- Next you will navigate down to "Boot Disk" and click the change button. This will take you to a page where you can select the OS and the version. Choose Windows Server as your operating system. The version chosen in this example is called Windows Server 2019 Datacenter. It is key to note that the version states it provides a desktop experience. Keep the other defaults and press select when you are done.

![](https://github.com/Samir-Sell/Cloud_Computing_Google/blob/main/Images/Desktop.png)

- Navigate to "Identity and API Access" and select "Allow full access to all cloud APIs". This will enable your VM to communicate with other Google Services such as Google Storage. Also ensure to tick off the Allow HTTP and HTTPS traffic boxes to ensure no functionality you may want to be blocked. 
- Click create and wait a few minutes for your VM to be generated. Please note that when it is created, it is enabled and you will begin to pay! 

## How to View your VM

- We are going to want a way to access desktop of the VM. We will need to download a piece of software that will allow us to remote desktop protocol into our machine. This tutorial will use MobaXterm. Please use this [link](https://mobaxterm.mobatek.net/download.html) to download the free version. Follow the steps prompted from you to complete your download. 
- Navigate to your VM instances page. If your VM instance is not running, start it by selecting it and then pressing the start button in the upper panel. Navigate to where your VM says RDP and click the dropdown menu beside it. You will now click on "Set Windows Password". It will prompt you for a username, I would reccommend choosing the default one it generates for you and clicking set. Google will then provide a password to you. Copy this and save it to safe location. 
- Open up MobaXterm and select the "New Session" button. Then go back to your Google VM instances page and copy the external IP address. Paste the external IP address into the remote host text box and then type your username into the username textbox. This is the user name you just created when creating a Windows password for your VM. You will now be prompted for your password that was generated for you. Enter this and wait for the VM to boot up. It may take a couple minutes. Voila! You now have a functional Google Compute Engine VM! 

## How to Set Up your Python Environment

- In order to take advantage of the computing power of the VM, we have to set up a development environment where we can run processes. We will want to install a more powerful and new age internet browser. In this example, I chose to download Google Chrome. To download Google Chrome, we have to use the default Internet Explorer browser that is installed on our machine. 
- Open up Internet Explorer on your VM and click the following: The gear option in the top right > Internet Options > Security > Custom Level > Scroll to file downloads and click enable > ok > apply
- Then Restart Internet Explorer and search up Google Chrome. Install Google Chrome. 
- Use Google Chrome to navigate to Anacondas [download page](https://www.anaconda.com/products/individual). Install the Windows 64 bit version and run the executable. Accept all the defaults except for in the advanced installation options. Make sure you tick off the box that states "Add Anaconda 3 to my PATH environment variable". The installation process may take a while. 
- Next we will install an Integrated Development Environment (IDE) we can use to write Python scripts. The IDE I have chosen is called Visual Studio Code. It can be found [here](https://code.visualstudio.com/). Follow the steps and install with the defaults.


Voila! You now have a fully functional VM that is set up for a Python Environment!


## Further Reading

[Anaconda Basics](https://docs.anaconda.com/anaconda/user-guide/getting-started/)
[More Anaconda](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html)



