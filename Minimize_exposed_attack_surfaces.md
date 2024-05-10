# 6. Minimize exposed attack surfaces 

The "principle of least privilege" is a fundamental concept in security engineering, crucial for IoT just as in any other area of application. 

## Provision 6.1  

**All unused network and logical interfaces shall be disabled.** 

> Example 1: An administrative UI that is supposed to be accessed from the LAN is not accessible from the WAN by default. 

> Example 2: A Direct Firmware Update (DFU) service exposed over Bluetooth® Low Energy is used for development but not expected to be used in production. It is disabled in the final product. 

## Provision 6.2 

**In the initialized state, the network interfaces of the device shall minimize the unauthenticated disclosure of security-relevant information.** 

During the initialization process, security-related details may be transmitted over a network interface. If this information is shared while establishing a connection, attackers could use it to pinpoint vulnerable devices. 

> Example: When finding vulnerable devices throughout the whole IP address space, security-relevant information could be information about the device configuration, kernel version or software version. 

## Provision 6.3 

**Device hardware should not unnecessarily expose physical interfaces to attack.** 

Attackers can exploit physical interfaces to compromise firmware or memory on a device. The term "unnecessarily" relates to the manufacturer's evaluation of the advantages of an open interface, which might be used for user features or debugging. 

## Provision 6.4 

**Where a debug interface is physically accessible, it shall be disabled in software.** 

> Example: A UART serial interface is disabled through the bootloader software on the device. No logon prompt and no interactive menu is available due to this disabling. 

## Provision 6.5  

**The manufacturer should only enable software services that are used or required for the intended use or operation of the device.** 

> Example: The manufacturer does not provision the device with any background processes, kernel extensions, commands, programs or tools that are not required for the intended use. 

## Provision 6.6  

**Code should be minimized to the functionality necessary for the service/device to operate.** 

> Example "Dead" or unused code is removed and not considered to be benign. 

## Provision 6.7 

**Software should run with least necessary privileges, taking account of both security and functionality.** 

> Example 1: Minimal daemons/processes run with "root" privileges. In particular the processes that use network interfaces require unprivileged users rather than requiring a "root" user. 

> Example 2: Applications running on a device that includes a multi-user operating system (e.g. Linux® ) use different users for each component or service. 

## Provision 6.8 

**The device should include a hardware-level access control mechanism for memory.** 

Software exploits frequently exploit the absence of access control in memory to run harmful code. Access control mechanisms restrict whether data in device memory can be executed. These mechanisms include technologies like Memory Management Units (MMUs) or Memory Protection Units (MPUs), executable space protection (e.g., NX bits), memory tagging, and trusted execution environments. 

## Provision 6.9  

**The manufacturer should follow secure development processes for software deployed on the device.** 

Employing secure development practices, such as utilizing version control and enabling security-related compiler options like stack protection, can enhance the security of software artifacts. Manufacturers should leverage these options when utilizing toolchains that support them.
