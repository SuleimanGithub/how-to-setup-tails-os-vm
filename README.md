# **How-to-setup-tails-os-vm**

#### Introduction: Welcome to the tutorial on creating a VirtualBox with TailsOS, Oracle VM VirtualBox is simple yet powerful as it can be run from a multitude of devices such as small embedded systems to datacenter deployments whilst TailsOS is a portable operating system that protects against surveillance and censorship.

___

## 1. Check that you have the required computer specification:

### *Hardware requirements:*

- Storage device: Minimum of 8 GB.

- Processor: A 64-bit x86-64 compatible.

- For optimal performance: 2 GB of RAM.

### *How can I check my system's hardware?*

- Click the Start button and type "system information" then open it.

- You can find most of the details you need on the first page, in the System Summary node.

- You can also expand each node in the left pane for additional information.
___

## 2. Setting up the VirtualBox:

### *What is a VirtualBox?*

- In short, VirtualBox is a tool developed by Oracle to allow running multiple operating systems simultaneously. This allows easier software installations, better testing, faster disaster recovery, and it significantly reduce hardware and electricity costs.  
The complete introduction can be found here:  
[virtualbox.org - Chapter 1. First Steps][1]

### *How to install the VirtualBox?*

- You can install VirtualBox by downloading the executable file for your operating system.  
The download page that can be found here:  
[virtualbox.org - Downloads][2]

---

## 3. Setting up Tails OS:

- Running Tails in a virtual machine is easy. First you need to download an ISO (Optical Disc Image) with the latest Tails Operating System (OS). This ISO image will be used to emulate inserting a CD to our VirtualBox to set up our Tails OS machine.  
The Tails OS ISO image can be found here:  
[tails.boum.org - Downloads][3]

### *Running Tails in a virtual machine:*

#### Start VirtualBox, and follow below instructions:

#### A) To create a new virtual machine:

1. Choose **Machine ▸ New**....
2. In the **Name and operating system screen**, specify:
   - A name of your choice.
   - Type: **Linux**.
   - Version: **Other Linux (64 bit)**.
   - Click **Next**.
3. In the **Memory size** screen:
   - Allocate at least 2048 MB of RAM.
   - Click **Next**.
4. In the Hard drive screen:
   - Choose **Do not add a virtual hard drive**.
   - Click **Create**.
   - Click _**Continue**_ in the warning dialog about creating a virtual machine without a hard drive.

#### B) To configure the virtual machine to start from our ISO image:

1. Select the new virtual machine in the left pane.
2. Choose **Machine ▸ Settings**....
3. Select **System** in the left pane.
4. In the **Extended Features** section of the **Motherboard** tab, make sure that **Enable I/O APIC** is enabled.
5. Select **Storage** in the left pane.
6. Select **Empty** below **Contoller IDE** in the **Storage Tree** selection list in the right pane.
7. Click on the **CD** icon on the right of the window and select **Choose a virtual CD/DVD disk file**... to browse for the ISO image you want to start Tails from.
8. Check the **Live CD/DVD** option.
9. Click **OK**.

#### C) To start the new virtual machine:

1. Select the virtual machine in the left pane.
2. Click **Start**.

That's about it! When complete you should see something like this:

![Virtual Box](TailsOSimagevs.jfif)
___

[1]: https://www.virtualbox.org/manual/ch01.html#virt-why-useful
[2]: https://www.virtualbox.org/wiki/Downloads
[3]: https://tails.boum.org/install/vm-download/index.en.html