# cybersecurity-home-lab

### Installing Kali Linux "Pre-Built Image" and VMware Workstation Pro.
Check out the **[kali-linux-installation-screenshots](kali-linux-installation-screenshots)** folder for all the screenshots.

## Kali Linux & Ubuntu Server on VMware Workstation Pro.
This project documents the step-by-step process of setting up a **cybersecurity home lab** using **VMware Workstation Pro**, with a detailed guide on downloading and installing Kali-Linux "pre-built image", Ubuntu server "installer image" and VMware Workstation Pro virtualisation tool. With these tools, you can simulate attacks using the Kali Linux VM and perform log analysis and monitoring on the Ubuntu server.   

## Project Overview
| Component                          | Purpose                                                                                   |
|------------------------            |-------------------------------------------------------------------------------------------|
| VMware Workstation Pro             | Virtualization platform.                                                                  |
| Kali Linux (OVA - Pre-Built Image) | Offensive security and pentesting, for penetration testing and vulnerability scanning.    |

Virtualization is the process of creating a virtual version of computing environments—such as operating systems, servers, and networks—on a single physical machine. It enables users to run multiple systems simultaneously, making it an essential tool for testing, development, and cybersecurity labs.

VMware Workstation Pro is a powerful virtualization software that allows users to run multiple virtual machines on a single physical system. It's widely used by IT professionals, developers, and cybersecurity analysts to simulate real-world environments without needing separate hardware.

Kali Linux is a Debian-based Linux distribution specifically designed for penetration testing and ethical hacking. Pre-loaded with hundreds of security tools, it’s a go-to OS for cybersecurity professionals and learners aiming to test vulnerabilities, perform digital forensics, and learn offensive security techniques in a controlled environment.

In this article, I’ll walk you through installing Kali Linux’s official pre-built image on VMware Workstation Pro—perfect for beginners and pros looking to quickly get hands-on with real-world security tools.

As of November 11, 2024, VMware Workstation Pro is free for personal use, which implies that a license key is no longer required during installation. The company “BROADCOM” completed the acquisition of VMware on November 22, 2023. VMware Workstation Pro became part of Broadcom's software portfolio at that time.

STEP 1: Log in to the Broadcom support website
Sign up or sign in to Broadcom Support Portal. If you already have an account, click on "Login"; otherwise, click on "Register" as pointed to by the second and first arrow, respectively.
**View: [step1A](kali-linux-installation-screenshots/step1A.png)**

Assuming you are registering for the first time, fill in your information as shown below. You are expected to enter the text from the image pointed to by the 2nd arrow into the box below it, pointed to by the 3rd arrow. If you are unsure about the text, you have the option to click on the speaker to hear the text read out loud as pointed to by the 4th arrow. You can also click the refresh button to change the given text as pointed to by the 5th arrow. Click on Next and follow through with the signup process.
**View: [step1B](kali-linux-installation-screenshots/step1B.png)**

After signing up successfully, log in to the portal.
**View: [shot1C](kali-linux-installation-screenshots/shot1C.png)**

STEP 2: Download VMware Workstation.
After logging in, you will be directed to the home page shown below:

The 1st arrow points to your registered name, showing you are logged in. Click on either of the links pointed to by the 2nd arrow and click on “VMware Cloud Foundation”, next click on “My Downloads”.
**View: [step2A](kali-linux-installation-screenshots/step2A.png)**

Click “HERE” pointed to by the 2nd arrow in the screenshot below.
**View: [step2B](kali-linux-installation-screenshots/step2B.png)**

Search by typing “VMware Workstation” inside the search bar as pointed to by the 1st arrow and click on “Show Results”. The matched results will be displayed, click on the “VMware Workstation Pro” as pointed to by the 3rd arrow.
**View: [step2C](kali-linux-installation-screenshots/step2C.png)**

Two operating systems versions of the VMware Workstation Pro are displayed, pointed to by the two arrows; choose the one that corresponds to your operating system. We are selecting the Windows OS version.
**View: [step2D](kali-linux-installation-screenshots/step2D.png)**

Click on the "caret" pointed to by the 1st arrow to expand the Windows OS “VMware Workstation Pro” version. Click on the latest version as pointed to by the 2nd arrow.
**View: [step2E](kali-linux-installation-screenshots/step2E.png)**

Click on the download button to start downloading the `VMware Workstation Pro`.
**View: [step2F](kali-linux-installation-screenshots/step2F.png)**

## Step 3: Install the VMware Workstation
Check your download folder or whichever location you specified for your downloads, and right-click on the executable file, click “Run as Administrator”

Follow through the remaining installation process using the arrows shown in the screenshots below.
**View: [step3A](kali-linux-installation-screenshots/step3A.png)**
**View: [step3B](kali-linux-installation-screenshots/step3B.png)**

I recommend you check the box pointed to by the 1st arrow, so you can be able to access your “VMware Workstation Pro” through the native computer Command Prompt. You can choose to change the default installation location by clicking on the “Change” button pointed to by the 3rd arrow and specifying your desired path/location. Click on "Next" after that.
**View: [step3C](kali-linux-installation-screenshots/step3C.png)**

Check the boxes and click on Next.
**View: [step3D](kali-linux-installation-screenshots/step3D.png)**

Check the boxes and click on Next.
**View: [step3E](kali-linux-installation-screenshots/step3E.png)**
**View: [step3F](kali-linux-installation-screenshots/step3F.png)**
**View: [step3G](kali-linux-installation-screenshots/step3G.png)**
**View: [step3H](kali-linux-installation-screenshots/step3H.png)**

## Step 4: Download the Kali Linux “pre-built image”.
We can use “Pre-built image (.7z archive)” or “Installer image (.iso file)” to run virtual machines on VMware Workstations. In this article, we are focusing on downloading the pre-built image. The “Installer image” has the most tedious installation process, where you have much control to specify installation settings.

Visit Kali Platforms, click on the “Virtual Machine” box as pointed to by an arrow. A “Pre-built Image” VM is an existing virtual machine, we can quickly start the VM immediately after we download it without going through any installation and configuration settings.
**View: [step4A](kali-linux-installation-screenshots/step4A.png)**

Because we are using the VMware virtualization platform, click on the VMware download button as pointed to by the 1st arrow, with the actual download size of "3.2G" written just beside it. You can see that besides VMware, there are other virtualization platforms like Oracle VirtualBox. The download starts immediately you click on it. After that,  locate the downloaded “archived file” and unzip it. Right-click on the file and click on "Extract File".
**View: [step4B](kali-linux-installation-screenshots/step4B.png)**

Step 5: Open the Kali Linux (pre-built image) in VMware Workstation Pro.
Double-click on the “VMware Workstation Pro” shortcut to open it. Remember the Kali Linux “pre-built image” is an existing Virtual Machine, on this premise,  click on the “Open a virtual machine” and locate the extracted file unzipped above.
**View: [step5A](kali-linux-installation-screenshots/step5A.png)**

Locate the extracted file, double click on it to automatically open it, or select it and click on open to open it on “VMware Workstation Pro”.
**View: [step5B](kali-linux-installation-screenshots/step5B.png)**

After opening the Kali-Linux Pre-built Image, you will be presented with the interface shown below. The 1st arrow points to the virtual machine name, the 2nd arrow points to the machine state, which is currently “powered off”. The two 3rd arrows point to the start button, you can click on the ‘caret’ symbol right beside the green button to view and use other options like “shutdown, suspend, or restart” the VM. The VM settings can be edited and also upgraded as pointed to by the 4th arrow. The 5th arrow points to the device information regarding Memory and processors allocated, among others, which are all subject to change using the "Edit virtual machine settings" pointed to by the 4th arrow. The 6th arrow points to all open tabs, where we have the “Home” and “kali-linux-2025.1a-vmware-amd64” tabs.
**View: [step5C](kali-linux-installation-screenshots/step5C.png)**

Click on the Start button as shown above, and enter the default username and password of “kali” to log in to the Kali Linux VM.
**View: [step5D](kali-linux-installation-screenshots/step5D.png)**

Voila,  we have successfully logged in to the Kali Linux VM.
**View: [step5E](kali-linux-installation-screenshots/step5E.png)**

We have successfully downloaded and installed both Kali Linux pre-built images and VMware Workstation Pro, and opened Kali Linux VM on VMware Workstation.

**NOTE**:
Alternatively to the Kali Linux “pre-built image”, you can choose to download and use the Kali Linux “Installer Images” instead, as shown below. The Kali Linux “Installer Images” enable you to create the Kali Linux VM from scratch, where you are responsible for specifying all the system configurations and settings, such as RAM allocation and storage location, among others.
**View: [step6A](kali-linux-installation-screenshots/step6A.png)**

Click on “Recommended,” and you will be directed to the download page shown below. Select your system processor architecture, where "x86_64" refers to the traditional 64-bit processor architecture commonly found in most PCs, while "Apple Silicon (ARM64)" is Apple's proprietary 64-bit processor architecture used in newer Mac computers.
**View: [step6B](kali-linux-installation-screenshots/step6B.png)**

The Installer Image is an “.iso” file, used to create virtual machines. After the download, open the VMware workstation, click on “Create a New Virtual Machine” and locate where the “.iso” file is downloaded and select it. Follow the on-screen prompts to proceed with the rest of the installations and settings. The default selections during the installation, in most cases, should work fine.
**View: [step6C](kali-linux-installation-screenshots/step6.png)**










## VMware and Kali Linux (Pre-Built Image) Installation Steps.
- STEP 1: Log in to the [Broadcom support](https://support.broadcom.com/) website.
- STEP 2: Download VMware Workstation.
- Step 3: Install the VMware Workstation.
- Step 4: Download the [Kali Linux](https://www.kali.org/get-kali/#kali-platforms) (`.ova` file) “pre-built image”.
- Step 5: Open the Kali Linux (pre-built image) in VMware Workstation Pro.
- 
## Ubuntu Server (Installer Image) Installation Steps.
- Step 1: Download Ubuntu Server [Installer Image](https://ubuntu.com/download/server) (`.iso` file).
- Step 2: Open VMware Workstation Pro and Create a New Ubuntu VM.
- Step 3: Start the Ubuntu Server created in VMware Workstation Pro.
- Step 4: Enable [Ubuntu-Pro](https://ubuntu.com/pro)  

## LinkedIn Article.
- [Installing Kali Linux Pre-built Image on VMware Workstation Pro](https://www.linkedin.com/pulse/installing-kali-linux-pre-built-image-vmware-workstation-enoch-agbu-qvuif)<br>
- [Installing Ubuntu-server Installer Image on VMware Workstation Pro](https://www.linkedin.com/pulse/installing-ubuntu-server-installer-image-vmware-workstation-agbu-pjidc)

## Connect with me.
[🔗 LinkedIn](https://www.linkedin.com/in/agbuenoch)<br>
[🔗 X](https://www.x.com/agbuenoch)
