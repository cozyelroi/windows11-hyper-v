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

![image](https://github.com/user-attachments/assets/7d3306d7-8351-4c5d-ae5e-20e40f2e1f5b)
![image](https://github.com/user-attachments/assets/2f618c45-f13c-4e4c-b84b-bcad9b8f8772)
![image](https://github.com/user-attachments/assets/a369d0eb-87a0-4e5f-92b1-3aade6cc1c3c)

2. Check the box for **Hyper-V** and click **OK**.
3. Restart the system if prompted to complete the Hyper-V installation.
![image](https://github.com/user-attachments/assets/51195264-50c8-4055-803d-00354a73600a)

### Step 2: Download the Windows 11 ISO
1. Download the **Windows 11 ISO** from the official Microsoft website: [Windows 11 Download](https://www.microsoft.com/en-us/software-download/windows11).
2. Save the ISO file to a location on the host machine.

### Step 3: Create a New Virtual Machine
1. Open **Hyper-V Manager**.
2. In the right pane, click **New** > **Virtual Machine**.
![image](https://github.com/user-attachments/assets/089384c8-bf1c-4199-9c3e-2354e8297b8d)

3. Follow the prompts in the wizard:
   - **Name** the virtual machine (e.g., "Windows 11 VM").
   ![image](https://github.com/user-attachments/assets/d345afa7-d6b7-427a-8d09-272f9aac2ae7)

   - Choose **Generation 2** for the virtual machine to enable secure boot and UEFI support.
![image](https://github.com/user-attachments/assets/fee12d9d-9b4b-4b0e-b86f-9d3f813176e1)

   - Assign **memory** (at least 4 GB) to the virtual machine.
![image](https://github.com/user-attachments/assets/37e14ed0-f8c0-4299-8691-adeeee6ec050)

   - Create a **virtual hard disk** (at least 64 GB recommended).
![image](https://github.com/user-attachments/assets/92a8c776-8820-475b-a044-1ffe22ae742d)

    - Choose **Install an operating system from a bootable CD/DVD-ROM**, and select the downloaded **Windows 11 ISO** file.
![image](https://github.com/user-attachments/assets/425e56f8-76b4-4b02-89e2-c06d81e56c9d)
![image](https://github.com/user-attachments/assets/e68026fe-ab69-4f24-a9c2-62f09fe6cb15)

### Step 4: Configure Virtual Machine Settings
1. After creating the virtual machine, right-click the VM and select **Settings**.
![image](https://github.com/user-attachments/assets/8ba1a61a-d042-4ee0-bf29-a4a573f060e4)

2. Under **Processor**, allocate at least 2 CPUs for optimal performance.
![image](https://github.com/user-attachments/assets/92524e4c-1ed5-410b-bad5-b16f63741687)

3. Under **Network Adapter**, select the virtual switch that connects the virtual machine to the host network.
![image](https://github.com/user-attachments/assets/413b0e9d-6f6d-4f2e-a0d2-ab3c2954f63c)

### Step 5: Start the Virtual Machine and Install Windows 11
1. Start the virtual machine by right-clicking on it and selecting **Start**.
![image](https://github.com/user-attachments/assets/66a5c977-fac8-4dfa-a5cd-537b8729c7cb)

2. Open the **VMConnect** window to interact with the virtual machine.
![image](https://github.com/user-attachments/assets/55b0ebb5-5e87-4637-a59e-d959d04cf9fe)
![image](https://github.com/user-attachments/assets/911855f8-00a9-41be-92fb-d2d8477418ca)

3. Follow the on-screen instructions to install **Windows 11**:
![image](https://github.com/user-attachments/assets/f80fc3ad-1add-44cd-99cd-13e894452359)
![image](https://github.com/user-attachments/assets/2a1c15c2-427d-4382-862c-87dca0c7fcf0)

   - Choose the language, time, and keyboard layout.
![image](https://github.com/user-attachments/assets/a47bc48c-0489-4531-af28-de48d1e6dd21)
![image](https://github.com/user-attachments/assets/f2aede55-469e-46a4-9dde-6b21937c8cc7)
![image](https://github.com/user-attachments/assets/f8926690-3087-458d-a1f5-27da107502e3)
![image](https://github.com/user-attachments/assets/b59c891c-ff15-4fdb-85bf-516e6ad92bd3)

5. Let the installation complete, which may take several minutes.


### Step 7: Complete the Setup and Final Configuration
1. Ensure that the virtual machine has internet access by verifying the network settings.

## Conclusion

This lab provided a comprehensive guide for setting up **Windows 11** in a **Hyper-V** virtual environment. The knowledge gained can be applied to various scenarios, such as testing new applications, developing in isolated environments, or running multiple OS versions for educational purposes. Understanding how to manage virtual machines in **Hyper-V** is a critical skill for system administrators, developers, and IT professionals working with virtualized infrastructure.

## Next Steps

- Explore the creation of more complex virtual environments with multiple VMs.
- Learn how to manage virtual machine snapshots and backup strategies.
- Configure additional networking settings for virtual machines in **Hyper-V**.

