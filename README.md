# documenting-a-technical-process-lab


# Setting Up an Ubuntu Virtual Machine on macOS Using VirtualBox

## Description
This guide explains how to:
1. Install VirtualBox on macOS
2. Set up VirtualBox to run Ubuntu 24.04
3. Configure Ubuntu VM with additional updates and features. 

---

## Part 1: Install VirtualBox on macOS

### Prerequisites for installtion
- macOS 10.14 or later
- Admin access to install apps (if you are using a standard account on macOS, the admin will need to inout there password to for installtion process)


### Steps

1. **Download VirtualBox**
   - - **Apple Silicon Macs (ARM)**: https://download.virtualbox.org/virtualbox/7.1.6/VirtualBox-7.1.6-167084-macOSArm64.dmg
   - **Apple Silicon Macs (ARM)**: https://download.virtualbox.org/virtualbox/7.1.6/VirtualBox-7.1.6-167084-OSX.dmg


2. **Install VirtualBox**
   - Open the `.dmg` file and run the installer.
   - Double-click the `VirtualBox.pkg icon`.
   - You will be given many prompts on features to install and choices to make while installing VB. Just accept all the default options.
   - When the installation is complete, you will see a message that says **_The installation was successful. Select the Close button._**
   - You can locate the VirtualBox application in your `Applications` directory

---

## Part 2: Set Up an Ubuntu 24.04 VM

### Step 1: Download the Ubuntu ISO

- **Intel Macs**:  
  [Download Ubuntu 24.04 ISO](https://ubuntu.com/download/desktop)

- **Apple Silicon Macs (ARM)**:  
  [Download Ubuntu 24.04 ARM ISO](https://ubuntu.com/download/arm)

- Note: This will take about an hour or so over stable internet

### Step 2: Create a New Virtual Machine

1. Open VirtualBox and click **New**.
2. Set up the following:
   - **Name**: `Ubuntu VM`
   - **Type**: `Linux`
   - **Version**:
     - Intel Macs: `Ubuntu 24.04 LTS (Noble Numbat) 64-bit`
     - Apple Silicon Macs: `Ubuntu 24.04 LTS (Noble Numbat) (ARM 64-bit)`
3. Click **Next**. 

### Step 3: You will arrive to tthe Hardware section

- **Base Memory**: Allocate at least **2048 MB(2 GB) of RAM** (4096 MB/4GB  is recommended for better performance)
- **Processors**: Minimum 1; 2 or more for better performance
- Click **Next**

### Step 4: Virtual Hard Disk section

1. Choose **Create a virtual hard disk now**
2. Move the bar or type:
   - Size: **32 GB recommended** (12 GB minimum)
3. Click **Next**
4. You will be taken to the **Summary** screen, click on **Finish**

### Step 5: Attach Ubuntu ISO (macOS-specific)

1. Select your VM, go to **Settings > Storage**
2. Selet on **Add Attachment** button. ( its a floppydisk icon with a green plus button)
3. Select **Optical Disk**. A new window wil open.
4. In the new window, select **Add** icon at the top of the window, and choose the **Ubuntu ISO** you downloaded earlier. Click on **Choose**
4. Once added on the previous screen, Click **OK**

### Step 6: Start and Install Ubuntu

1. VM should now appear in the VirtualBox Manager. Select the VM and click **Start**
2. Ubuntu will boot from the ISO
3. Follow the Ubuntu's installer prompts:
   - Select your keyboard layout and installation type
   - Create user account and password for Ubuntu
   - Wait for installation to complete
4. Reboot the VM when prompted, so the confirguations are saved. 


_You have successfully installed VirtualBox and Ubuntu as your first Vm!!!_ 

---




