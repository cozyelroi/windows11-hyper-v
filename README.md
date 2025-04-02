# Lab: Installing Windows 11 in Hyper-V

## Lab Overview

This lab focuses on installing **Windows 11** within **Hyper-V**, Microsoft’s virtualization platform. The steps outlined will guide through the process of setting up a virtual machine (VM) for Windows 11, configuring necessary resources, and completing the installation. The ability to deploy virtualized environments is crucial for testing, development, and educational purposes.

### Who
This lab is intended for IT professionals, system administrators, and anyone interested in learning how to set up virtual machines in a Hyper-V environment. It is also useful for individuals seeking to test or develop software in an isolated environment.

### What
In this lab, the following tasks will be performed:
- Create a new virtual machine in Hyper-V.
- Allocate resources (CPU, RAM, Storage) to the virtual machine.
- Install Windows 11 on the virtual machine.
- Configure the virtual machine’s networking settings and integration services.

### When
This lab can be conducted at any time and is suitable for both beginners and intermediate users with an understanding of virtualization concepts.

### Where
The lab is performed using **Hyper-V**, which can be set up on a Windows machine running **Windows 10 Pro**, **Windows 11 Pro**, or a **Windows Server** edition that supports Hyper-V.

### Why
Setting up Windows 11 in Hyper-V is beneficial for testing new features, running legacy applications, or developing and isolating environments without impacting the host operating system. This lab provides the skills to work with virtual machines and expand capabilities in system administration, testing, and troubleshooting.

## Prerequisites

- A host machine running **Windows 10 Pro**, **Windows 11 Pro**, or a **Windows Server** edition that supports Hyper-V.
- Access to a **Windows 11 ISO** file.
- **Hyper-V** enabled on the host machine.
- Basic understanding of virtualization and virtual machines.

## Lab Goals

- Set up a virtual machine in **Hyper-V**.
- Install **Windows 11** within the virtual machine.
- Configure the virtual machine’s hardware and network settings.
- Learn how to manage virtual machines in Hyper-V.

## Steps

### Step 1: Enable Hyper-V on the Host Machine
1. Open **Control Panel** > **Programs** > **Turn Windows features on or off**.
2. Check the box for **Hyper-V** and click **OK**.
3. Restart the system if prompted to complete the Hyper-V installation.

### Step 2: Download the Windows 11 ISO
1. Download the **Windows 11 ISO** from the official Microsoft website: [Windows 11 Download](https://www.microsoft.com/en-us/software-download/windows11).
2. Save the ISO file to a location on the host machine.

### Step 3: Create a New Virtual Machine
1. Open **Hyper-V Manager**.
2. In the right pane, click **New** > **Virtual Machine**.
3. Follow the prompts in the wizard:
   - **Name** the virtual machine (e.g., "Windows 11 VM").
   - Choose **Generation 2** for the virtual machine to enable secure boot and UEFI support.
   - Assign **memory** (at least 4 GB) to the virtual machine.
   - Create a **virtual hard disk** (at least 64 GB recommended).
   - Choose **Install an operating system from a bootable CD/DVD-ROM**, and select the downloaded **Windows 11 ISO** file.

### Step 4: Configure Virtual Machine Settings
1. After creating the virtual machine, right-click the VM and select **Settings**.
2. Under **Processor**, allocate at least 2 CPUs for optimal performance.
3. Under **Network Adapter**, select the virtual switch that connects the virtual machine to the host network.

### Step 5: Start the Virtual Machine and Install Windows 11
1. Start the virtual machine by right-clicking on it and selecting **Start**.
2. Open the **VMConnect** window to interact with the virtual machine.
3. Follow the on-screen instructions to install **Windows 11**:
   - Choose the language, time, and keyboard layout.
   - Enter a valid product key (optional, for evaluation purposes).
   - Select the partition to install **Windows 11** (use the default disk).
4. Let the installation complete, which may take several minutes.

### Step 6: Install Integration Services (Optional)
1. After the installation of Windows 11 is complete, install **Hyper-V Integration Services** by going to **Action** > **Insert Integration Services Setup Disk**.
2. Run the setup to enhance the performance and integration of the virtual machine with the host system.

### Step 7: Complete the Setup and Final Configuration
1. Configure Windows 11 settings (e.g., user account, password, region, etc.).
2. Ensure that the virtual machine has internet access by verifying the network settings.

## Conclusion

This lab provided a comprehensive guide for setting up **Windows 11** in a **Hyper-V** virtual environment. The knowledge gained can be applied to various scenarios, such as testing new applications, developing in isolated environments, or running multiple OS versions for educational purposes. Understanding how to manage virtual machines in **Hyper-V** is a critical skill for system administrators, developers, and IT professionals working with virtualized infrastructure.

## Next Steps

- Explore the creation of more complex virtual environments with multiple VMs.
- Learn how to manage virtual machine snapshots and backup strategies.
- Configure additional networking settings for virtual machines in **Hyper-V**.

