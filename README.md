# Graded Assignment on Networking and Server

# Task 1:
Deploy a website on localhost using either apache2 or Nginx. Create a DNS name for this website as ‘awesomeweb’. You can use any web template you want or can write your own simple HTML code.

[Solution](SolutionToTask1.md)


# Task 2:
A website can have many subdomains and different services are running on them. Write a Python script to check the status of the subdomains which are up or down. The script should automatically check the status every minute and should update it in tabular format on the screen. 

[Solution](SolutionTask2.md)

# Task 3:
Virtual Machine (VM) - Overview 

A virtual machine (VM) is a software emulation of a physical computer that runs an operating system and applications just like a physical machine. VMs allow you to create multiple isolated environments on a single physical host, each with its own virtual hardware configuration. This virtualization technology provides several advantages, such as the ability to run multiple operating systems on a single physical machine, easy migration of VMs between different hosts, and improved resource utilization. 

The virtualization layer called the hypervisor, is responsible for managing the VMs and enabling communication between them and the underlying physical hardware. There are two types of hypervisors: Type 1 hypervisor (bare-metal) runs directly on the physical hardware, while Type 2 hypervisor runs on top of an existing operating system. 

Oracle VirtualBox - Overview 

Oracle VirtualBox is a popular Type 2 hypervisor that allows you to create and manage virtual machines on your desktop or laptop. It supports a wide range of guest operating systems, including Windows, Linux, macOS, and more. VirtualBox is free and open-source, making it an excellent choice for developers, testers, and anyone interested in exploring virtualization. 

How to Install VirtualBox 

Here's a step-by-step guide to installing Oracle VirtualBox on your Windows, macOS, or Linux computer: 

Step 1: Download VirtualBox 

1. Go to the official VirtualBox website: https://www.virtualbox.org/ 

2. Click on the "Downloads" link in the top navigation menu. 

Step 2: Choose the Correct Package 

1. On the Downloads page, you'll see various packages for different host operating systems. Select the appropriate package for your OS (e.g., Windows, macOS, or Linux). 

Step 3: Install VirtualBox

1. For Windows: 

- Download the installer for Windows and double-click on the downloaded file to start the installation. 

- Follow the on-screen instructions and accept the license agreement. - Choose the components you want to install and the installation path. - Complete the installation process. 

2. For macOS: 

- Download the macOS version of VirtualBox. 

- Double-click on the downloaded DMG file to open it. 

- Double-click on the VirtualBox package icon to start the installation. - Follow the on-screen instructions to complete the installation. 

3. For Linux: 

- Download the appropriate package for your Linux distribution (e.g., .deb for Debian/Ubuntu-based systems, .rpm for Red Hat/Fedora-based systems). - Install VirtualBox using the package manager of your Linux distribution. For example, for Ubuntu, use the following command in the terminal: 

sudo dpkg -i <VirtualBox_package_name>.deb 

- You may need to install additional dependencies if prompted by the package manager. 

Step 4: Post-installation Configuration (All Operating Systems) 

1. After installation, you might need to add your user account to the "vboxusers" group (Linux) or "VirtualBox Users" group (Windows) to grant permissions to manage VMs. 

Step 5: Launch VirtualBox 

1. Once the installation is complete, you can launch VirtualBox from your application menu (Windows and Linux) or from the Applications folder (macOS). 

Congratulations! You now have Oracle VirtualBox installed on your computer and can start creating and managing virtual machines for various purposes, including development, testing, and exploration of different operating systems.

Once the VM has been installed, visit https://www.osboxes.org/ download a Ubuntu 22.04 image and start it through your VirtualBox. 

Install Nginx inside the Ubuntu machine and host a website. 

Come back to your host machine (windows/Linux/mac) and scan the virtual machine using Nmap. Create the documentation of the process and the output of the scan. Observe the ports which are open.


[Solution](SolutionToTask3.md)


