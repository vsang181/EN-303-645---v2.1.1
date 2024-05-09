## 3 Keep Software Updated

The most important action that can be taken by a manufacturer is timely development and deployment of security updates.

**Provisions 3.3 to 3.12 are dependent upon an update mechanism being implemented, as per provisions 3.1 or 3.2.**

### Provision 3.1 

**All software components in consumer IoT devices should be securely updateable.**

> Managing software updates successfully generally relies on communication of version information for software components between the device and the manufacturer.

But to mention not all software device can or will be updateable.

> Example 1: The first stage boot loader on a device is written once to device storage and from then on is immutable.

> Example 2: On devices with several micro controllers (e.g. one for communication and one for the application) some of them might not be updateable.

### Provision 3.2
 
**If case where device is not a constrained there should be an well defined mechanism for the installation of updates.**

> here are cases where provision 3.1 applies even where 3.2 does not.

"Securely updateable" and "secure installation" means that there are adequate measures to prevent an attacker misusing the update mechanism.

> Example 1: Measures can include the use of authentic software update servers, integrity protected communications channels, verifying the authenticity and integrity of software updates. It is recognized that there are great variances in software update mechanisms and what constitutes "installation".

> Example 2: An anti-rollback policy based on version checking can be used to prevent downgrade attacks.

Update mechanisms can range from the device downloading the update directly from a remote server, transmitted from a mobile application or transferred over a USB or other physical interface. 
 
### Provision 3.3

**An update shall be simple for the user to apply.**

The design and intended usage defines the degree of simplicity in this case. If an update is difficult to apply, then that increases the chance that a user will repeatedly defer updating the device, leaving it in a vulnerable state.

### Provision 3.4

**Automatic mechanisms should be used for software updates.**

Sometimes, if an automatic update fails, your device might stop working. But there are ways to detect and fix this, like using watchdogs or backup systems.

Security updates can stop hackers from exploiting weaknesses in your device. It's important for companies to have a clear plan to give you these updates and to let you know what's going on.

When companies release updates, they often rely on other companies for parts. But that shouldn't stop them from giving you updates. They should think about everyone involved in making the software safe.

It's usually better to keep security updates separate from big updates that add new features. Adding new stuff can make it harder to fix security problems quickly.

> Example: Under the EU Product Legislation, a feature update could change the intended use of a device and thus turn it into a new product, requiring a new conformity assessment to be conducted. However, a software update with limited impact could be considered a maintenance update which would not require a new conformity assessment. More information on the impact of software updates in the context of the EU Product Legislation can be found in the Blue Guide 

### Provision 3.5

**The device needs to regularly check if there are any security updates available, starting from when it's turned on and then at regular intervals afterwards.**

> Example 1: The user could be shown the existence of updates via the interface with which the device is initialized.

> Example 2: A device checks for available updates daily at a randomized time.

### Provision 3.6

**If the device can automatically update itself or notify you about updates, these features should be turned on when you first set up the device. You should also be able to choose whether you want to enable, disable, or delay the installation of security updates and notifications.**

Users should have the freedom to decide if they want to receive updates or not. There are valid reasons why someone might choose not to update, like concerns about security. Also, if an update causes problems, the company might ask users not to install it to avoid those issues. This puts control in the hands of the users and respects their rights and ownership of the device.

### Provision 3.7

**The device will employ advanced encryption methods to ensure that update processes are secure and protected from unauthorized access or tampering.**

### Provision 3.8

**Security updates shall be timely.**

"Timely" delivery of security updates can differ based on factors like the severity of the issue and the ability to reach affected devices, especially those with limited resources. Critical vulnerabilities, which could have widespread negative impacts, should be addressed urgently by the manufacturer. Because software today involves many parties and communication channels, coordinating security updates can involve multiple stakeholders.

> Example: A particular software update involves a third party vendor of software libraries, an IoT device manufacturer, and an IoT service platform operator. Collaboration between these stakeholders ensures appropriate timeliness of the software update.

### Provision 3.9

**The device should verify the authenticity and integrity of software updates.**

To make sure an update is safe, it's important to check if it's genuine and hasn't been tampered with. But some devices have limited power, so they might need help from another trusted device to do this check. Once confirmed, the update can be sent securely to the device, reducing the chance of hacking.

If an update is found to be fake or harmful, the device should not install it and should alert the right people. Steps can also be taken to stop attackers from tricking the update system. Giving as little detail as possible in the update process makes it harder for them to exploit it.

> Example: When a device detects that an update could not be delivered or applied successfully (by failing integrity or authentication checks), the device can mitigate information leakage by not providing any information about the failure to the initiator of the update process. However, the device can generate a log entry and deliver notification of the log entry to a trusted peer (e.g. a device administrator) over a secure channel, so that the occurrence of the incident is known and the owner or administrator of the device can make an appropriate response.

### Provision 3.10

**Where updates are delivered over a network interface, the device shall verify the authenticity and integrity of each update via a trust relationship.**

> alid trust relationships include: authenticated communication channels, presence on a network that requires the device to possess a critical security parameter or password to join, digital signature based verification of the update, or confirmation by the user

> he validation of the trust relationship is essential to ensure that a non-authorized entity (e.g. device management platform or device) cannot install malicious code.

### Provision 3.11

**The manufacturer should inform the user in a recognizable and apparent manner that a security update is required together with information on the risks mitigated by that update.**

> Example: The manufacturer informs the user that an update is required via a notification on the user interface or via an email.

### Provision 3.12

**The device should notify the user when the application of a software update will disrupt the basic functioning of the device.**

> This is not necessary if a notification is made by an associated service.

This notification can include extra detail, such as the approximate expected duration for which the device will be offline.

> Example 1: A notification includes information about the urgency and approximate expected duration of downtime.

It's really important that your device keeps working even when it's updating. That's why it's suggested to let you know if an update might interrupt how your device works. Especially for devices that are important for safety, they shouldn't just shut down during an update. They should still be able to do basic things to keep you safe. If updates aren't managed well, it could be a big safety problem for some devices.

> Example 2: During an update, a watch will continue to display the time, a home thermostat will continue to maintain a reasonable temperature and a Smart Lock will continue to lock and unlock a door.

### Provision 3.13

**The manufacturer shall publish, in an accessible way that is clear and transparent to the user, the defined support period.**

When purchasing a product, the consumer expects this period of software update support to be made clear.

### Provision 3.14

**For constrained devices that cannot have their software updated, the rationale for the absence of software updates, the period and method of hardware replacement support and a defined support period should be published by the manufacturer in an accessible way that is clear and transparent to the user.**

### Provision 3.15

**For constrained devices that cannot have their software updated, the product should be isolable and the hardware replaceable.**

Sometimes, certain devices can't be fixed with patches. For devices with limited capabilities, there should be a plan to replace them, and this plan should be clearly explained to users. The plan would usually include when you might need to get new devices and when the support for the current hardware and software will end.

### Provision 3.16

**The model designation of the consumer IoT device shall be clearly recognizable, either by labelling on the device or via a physical interface.**

This is often performed by communicating with a device over a logical interface, however it can also be part of a UI.

> Example: A device has a HTTP (or HTTPS when appropriate) API that reports the model designation (after user authentication).

Knowledge of the specific designation of the device is often required to check the defined support period of software
updates or the availability of software updates.

## Let's Connect

I welcome your insights, feedback, and opportunities for collaboration. Together, we can make the digital world safer, one challenge at a time.

- **LinkedIn**: (https://www.linkedin.com/in/aashwadhaama/)

I look forward to connecting with fellow cybersecurity enthusiasts and professionals to share knowledge and work together towards a more secure digital environment.
