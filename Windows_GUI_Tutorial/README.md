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

- We are going to want a way to access desktop of the VM. We will need to download a piece of software that will allow us to remote desktop protocol into our machine. This tutorial will use MobaXterm. Please use this [link](https://mobaxterm.mobatek.net/download.html) to download the free version. 
