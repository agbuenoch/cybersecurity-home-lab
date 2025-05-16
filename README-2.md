# cybersecurity-home-lab

## Installing Ubuntu Server "Installer Image" On VMware Workstation Pro.
Check out the **[ubuntu-server-installation-screenshots](ubuntu-server-installation-screenshots)** folder for all the screenshots.
 
## Project Overview
| Component                     | Purpose                                                                                               |
|------------------------       |-------------------------------------------------------------------------------------------------------|
| VMware Workstation Pro        | Virtualization platform.                                                                              |
| Ubuntu Server (`ISO` file)    | Server OS for SIEM and log analysis tools, as a base for detection tools like Wazuh, ELK, and Splunk. |

This project walks you through how to manually download and install Ubuntu Server "Installer Image”, an `.iso` file to create an Ubuntu server VM and specify its basic settings and configurations in `VMware Workstation Pro`.

## Step 1: Download the Ubuntu Server Installer Image.
Click [Ubuntu Server](https://ubuntu.com/download/server) to download the `installer image` for `Ubuntu 24.04.2 LTS`. `LTS` stands for Long-Term Support, which means five years of free security and maintenance updates, extended to `10 years` with [Ubuntu Pro](https://ubuntu.com/pro) if enabled. This means Ubuntu Pro delivers 10 years of expanded security coverage on top of Ubuntu’s Long Term Support (LTS) commitment, in addition to management and compliance tooling. After installing the installer image, we will enable `Ubuntu Pro`, which is free for personal use.

> NOTE: The arrows are sequentially numbered for easy understanding of the sequential steps to follow. Some of the directions the arrow points at are not links, but just to draw your attention to key observables.

**View: [step1A](ubuntu-server-installation-screenshots/step1A)**

The download will start immediately after you click on the download button, and you will be redirected to the page below.<br>
**View: [step1B](ubuntu-server-installation-screenshots/step1B)**

While the download is in progress, scroll downward and click on Get Ubuntu Pro, or you can visit the Ubuntu Pro website here to register for free. Click on the “Get Ubuntu Pro” as pointed to by the 3rd arrow.<br>
**View: [step1C](ubuntu-server-installation-screenshots/step1C)**

Click on “**Get Ubuntu Pro Now**” as pointed to by the 3rd arrow.<br>
**View: [step1D](ubuntu-server-installation-screenshots/step1D)**

Check the “**Myself**” button as pointed to by the 1st arrow and click on “**Register**” as pointed to by the 2nd arrow.<br>
**View: [step1E](ubuntu-server-installation-screenshots/step1E)**

If you don't have an account, check the first button; otherwise, check the second button as pointed to by the 1st and 2nd arrows respectively, and provide your details accordingly.<br>
**View: [step1F](ubuntu-server-installation-screenshots/step1F)**

After you sign in, copy down the “**Token**” pointed to by the 3rd arrow; we will use it to upgrade the Ubuntu server to “**Ubuntu Pro**” when we successfully create the Ubuntu server on the VMware Workstation Pro. The 4th arrow points to the command we should use to enable Ubuntu Pro.<br>
**View: [step1G](ubuntu-server-installation-screenshots/step1G)**

If you subsequently want to view your Token, visit ubuntu.com and click on "**Sign in**" at the top right-hand corner of the home page, and you will be redirected to the Ubuntu One Account Page. If this is the first time you're visiting ubuntu.com, you will be prompted with the cookie pop-up below, You can accept by clicking “**Accept all and visit site**” or choose to manage your preference by clicking the “**Manage your tracker settings**”.<br>
**View: [step1G2](ubuntu-server-installation-screenshots/step1G2)<br>**
**View: [step1H](ubuntu-server-installation-screenshots/step1H)**

You will be redirected to the page below. Provide your login details and click on “**Log in**”.<br>
**View: [step1H1](ubuntu-server-installation-screenshots/step1H1)**

Click the "**Yes, log me in**"<br>
**View: [step1H2](ubuntu-server-installation-screenshots/step1H2)**

Suppose you previously “**Accepted the cookie pop-up**”, the next time you click on "**Log in**", you won't be asked to enter your username and password again. In that case, you will be redirected to the screenshot immediately above, and you can click on the “**Yes, log me in**” because the cookie saved your login details and remembered you.

You have successfully logged in. You will then be redirected to this page, click on the “caret” symbol and click on the “**Ubuntu Pro dashboard**” as pointed to by the 1st and 2nd arrows, respectively.<br>
**View: [step1H3](ubuntu-server-installation-screenshots/step1H3)**

## Step 2: Open VMware Workstation and Create a New Ubuntu VM
Because the Ubuntu Server Installer Image is an `.iso` file, click on “Create a New Virtual Machine” as pointed to by the arrow. Follow the remaining installation process using the arrows as a guide.<br>
**View: [step2A](ubuntu-server-installation-screenshots/step2A)<br>**
**View: [step2B](ubuntu-server-installation-screenshots/step2B)**

The path to the downloaded `.iso` file is automatically detected, but if you changed the location, you can click on "**Browse**" as pointed to by the 2nd arrow to the new location where you kept the .iso file.

If you prefer to install the operating system later after creating the Ubuntu Server Virtual Machine, you can alternatively choose to check the button as pointed to by the 3rd arrow; otherwise, stick to the default selection as pointed to by the 1st arrow.<br>
**View: [step2C](ubuntu-server-installation-screenshots/step2C)**

Give the Ubuntu server a name of your choice as pointed to by the 1st arrow; you will be guided on acceptable syntax for your choice of names, for example, the use of upper case letters is not allowed.

You can also choose to change the location where the VM should reside by clicking on the "**Browse**" button as pointed to by the 2nd arrow; otherwise, click "**Next**".<br>
**View: [step2D](ubuntu-server-installation-screenshots/step2D)**

As pointed out by the 1st arrow, assign the disk size; `20GB` is the minimum size recommended.<br>
**View: [step2E](ubuntu-server-installation-screenshots/step2E)**

Click on the “Customise Hardware” as pointed to by the 1st arrow only if you want to change any settings or configuration. Changes can still be made even after the installation.<br>
**View: [step2F](ubuntu-server-installation-screenshots/step2F)**

When you click on “**Finish**”, you will be presented with the VM interface shown below. The 1st arrow points to the “**Play/start**” button used for powering the VM. Click on the “caret” symbol for other options like “Suspend, and Restart” buttons. You can edit the VM settings/configurations by clicking on the link pointed to by the 3rd arrow.<br>
**View: [step2G](ubuntu-server-installation-screenshots/step2G)**

## Step 3: Start the Ubuntu Server
From the screenshot above, start the Ubuntu server by clicking on the green play button pointed by the first or second arrow.

**NOTE**: 
> The arrows in the screenshots provided in the `Step 3` are not in sequential order. I will explain each one of them that is necessary.
Use the mouse to scroll up and down the VM interface, using the `scroll bar`. 
At this stage, you will start navigating between your native machine/host and the Ubuntu server VM. On your native machine keyboard, press “Ctrl G” or move the mouse cursor directly inside the VM and click inside it, to move/direct your keyboard input into the VM, this will enable you to interact with the VM directly using the keyboard which is very important especially at this installation process of starting the Ubuntu Server for the first time. While the keyboard focus is on the VM, press `Ctrl Alt` or move the mouse to click anywhere outside the VM, to move/direct the keyboard input out of the VM to the native machine.
Always scroll downward to accept the setting you have checked or selected. I used arrows to point to the scroll bar at the extreme right side of the window.

**View: [step3A](ubuntu-server-installation-screenshots/step3A)**

Press `Ctrl G` to direct keyboard input to the VM, and press "**Enter**" on your keyboard to activate the highlighted choice as pointed to by the 1st arrow. Do this for all other ones.<br>
**View: [step3B](ubuntu-server-installation-screenshots/step3B)<br>**
**View: [step3C](ubuntu-server-installation-screenshots/step3C)**

If you want to change your keyboard layout from the default one detected “**[English US]**” you can move the mouse to “Identify Keyboard” and press Enter on your keyboard, as pointed to by the 2nd arrow, otherwise just scrow down and press Enter when the mouse is on “**Done**”.<br>
**View: [step3D](ubuntu-server-installation-screenshots/step3D)**

Suppose you chose to “**Identify Keyboard**”. In that case, you will be asked a couple of questions, which I sample just two screenshots below, answer them accordingly, and your keyboard layout will be automatically detected.<br>
**View: [step3E](ubuntu-server-installation-screenshots/step3E)<br>**
**View: [step3F](ubuntu-server-installation-screenshots/step3F)<br>**
**View: [step3G](ubuntu-server-installation-screenshots/step3G)**

After the keyboard layout settings, the next steps follows. Move the mouse to activate/select the "**Ubuntu Server**" as pointed to by the 3rd arrow. The `X` inside the parentheses means it has been selected or activated, scroll downward as pointed to by the 2nd arrow, direct the mouse input back to the VM, ensure the mouse is active on “**Done**”, and press Enter.<br>
**View: [step3H](ubuntu-server-installation-screenshots/step3H)**

In the "**Network configuration**", scroll downward and press Enter while on "**TBD**"<br>
**View: [step3I](ubuntu-server-installation-screenshots/step3I)<br>**
**View: [step3J](ubuntu-server-installation-screenshots/step3J)<br>**

Skip the proxy configuration, scroll down, and press Enter while on the “**Done**” button.<br>
**View: [step3K](ubuntu-server-installation-screenshots/step3K)<br>**
**View: [step3K2](ubuntu-server-installation-screenshots/step3K2)**

Scroll downward and press Enter.<br>
**View: [step3L](ubuntu-server-installation-screenshots/step3L)**

Select “**Use an entire disk**” as pointed to by the 2nd arrow. The `X` means it is selected.<br>
**View: [step3M](ubuntu-server-installation-screenshots/step3M)<br>**
**View: [step3M2](ubuntu-server-installation-screenshots/step3M2)**

You will be presented with the storage configuration summary, scroll down and press Enter when you are active on the “**Done**” button.<br>
**View: [step3N](ubuntu-server-installation-screenshots/step3N)<br>**
**View: [step3N2](ubuntu-server-installation-screenshots/step3N2)<br>**
**View: [step3O](ubuntu-server-installation-screenshots/step3O)**

You will be prompted to click on “**Continue**”<br>
**View: [step3P](ubuntu-server-installation-screenshots/step3P)**

The next is “Profile Configuration”, provide the following details to sign up for login into the Ubuntu server after the installation. Use the "Tab" key on your keyboard to move from one row to another after entering the values.<br>
**View: [step3Q](ubuntu-server-installation-screenshots/step3Q)**

Select the “**Skip Ubuntu Pro setup for now**” and scroll down the cursor to “**continue**” and press Enter.<br>
**View: [step3R](ubuntu-server-installation-screenshots/step3R)**

Select the “**Install OpenSSH server**” as pointed to by the arrow below. Ensure you see `X` appear inside the bracket, scroll down and press Enter on “**Done**”.<br>
**View: [step3S](ubuntu-server-installation-screenshots/step3S)**

The installation process will begin; this will take a considerable number of hours, depending on your native machine specifications. The higher RAM and processor cores you have, the faster the installation process.

When you are running out of battery or internet connectivity at any stage of the installation especially this stage, I recommend you do not shut down your system or “**power off**” the VM or exit the VMware Workstation Pro, you should put your system on “**sleep**” mode and wake it up later when you have internet connections or charged your battery, to continue the installation process. Just remember, this process can take a while.<br>
**View: [step3T](ubuntu-server-installation-screenshots/step3T)<br>**
**View: [step3T2](ubuntu-server-installation-screenshots/step3T2)<br>**
**View: [step3U](ubuntu-server-installation-screenshots/step3U)**

Now "**shut down**” the Ubuntu server. Click on the “**caret**” symbol as pointed by the 1st arrow, you will see “**Shut Down Guest**” as pointed to by the 2nd arrow, click on it.<br>
**View: [step3V](ubuntu-server-installation-screenshots/step3V)**

After you shut down the VM, you will see the VM interface shown below, click on the "**CD/DVD (SATA)**", so that we can detach the `.iso` file installation directory from our native machine.<br>
**View: [step3W](ubuntu-server-installation-screenshots/step3W)**

As pointed out by the 1st arrow, uncheck the “**Connect at power on**” button. Checked the “**Use physical drive**” as pointed to by the 2nd arrow. Click on the “**caret**” symbol pointed to by the 3rd arrow and select “**Auto detect**”, scroll down as pointed to by the 4th arrow and click on “**ok**”.<br>
**View: [step3X](ubuntu-server-installation-screenshots/step3X)**

Now, “**Power on**” the Ubuntu server again by clicking on the green power button right in the VM interface. This time, the server will not load directly from the `.iso` file on our local machine. This will also take a while, just as indicated on the screenshot below.
**View: [step3Y](ubuntu-server-installation-screenshots/step3Y)**

You will be prompted to log in to the Ubuntu server using the signup details provided during the installation process above in “**Profile Configuration**”. Enter your username as pointed to by the 1st arrow, press “**Enter**” on your keyboard and enter the password as pointed to by the 2nd arrow. 

Voila! We have successfully logged in to the Ubuntu server and received a welcome message to “**Ubuntu 24.04.2 LTS**”. The 3rd arrow points to the message that says `ESM - i.e Extended Security Maintenance is not enable`. This is referring to the “**Ubuntu Pro**” and we will enable this feature in the next step so that we can receive additional future security updates up to 10+ years. After the welcome message and other additional information, we are presented with a “**Prompt**” to interact with the Ubuntu server. Let's explain the entire components of the “**Prompt**”. The 4th arrow points to the username, i.e the user currently logged in to the server. The 5th arrow points to the host/machine name, which is “ubuntu-server”; this is the name given to this Ubuntu server VM. The 6th arrow points to the dollar sign `$`, which refers to a normal user with less privileges. If this were an administrator or super user, the symbol or sign would be a hash sign `#`, which means the logged-in user would have a root user privilege.<br>
**View: [step3Z](ubuntu-server-installation-screenshots/step3Z)**

##  Step 4: Enable Ubuntu-Pro
Copy the token assigned to you when registering for “**Ubuntu Pro**” as demonstrated above, and run the command shown below. You will be required to provide a password for the user who is currently logged in to this server, this is to ensure the command is run by an authorized user.<br>
**View: [step4A](ubuntu-server-installation-screenshots/step4A)**

As pointed out by the arrow below, our `Extended Security Maintenance - ESM` is now enabled, which implies that the “**Ubuntu Pro**” is now enabled and attached to our Ubuntu server.<br>
**View: [step4B](ubuntu-server-installation-screenshots/step4B)**

## LinkedIn Article.
- [Installing Ubuntu-server Installer Image on VMware Workstation Pro](https://www.linkedin.com/pulse/installing-ubuntu-server-installer-image-vmware-workstation-agbu-pjidc)

## Connect with me.
[🔗 LinkedIn](https://www.linkedin.com/in/agbuenoch)<br>
[🔗 X](https://www.x.com/agbuenoch)
