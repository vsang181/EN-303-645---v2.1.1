## 1. No universal default passwords 

### Provision 1.1  

**Where passwords are used and, in any state, other than the factory default, all consumer IoT device passwords shall be unique per device or defined by the user.**

> Multiple ways can be used to perform authentication and authentication is not limited to passwords. But when the passwords are used [NIST Special Publication 800-63B](https://pages.nist.gov/800-63-3/sp800-63b.html) 

As a majority of IoT devices in the markets come with default credentials (such as “admin”:”admin”). Which have led to multiple accounts of security incidents. And this practice of default credentials has an absolute need to be discontinued. It can be remediated by using giving default pre-install credentials which are completely unique per device or by forcing the user/entity to change them before being able to use any functionality of the device or maybe using password independent methods. 

> Example: During initialization a device generates certificates that are used to authenticate a user to the device via an associated service like a mobile application. 

A multi factor authentication method could be used for better security implementation. 

### Provision 1.2 

**This is a provision where pre-initialized credentials are used and these should be generated with a mechanism that reduces the risk of automated attacks against a class or type of device.** 

> Example: Pre-installed credentials are sufficiently randomized. 

A pattern of passwords like “Password1”, “Password2”, “Password3” are easily recognizable. Also parameters sent over the same network or over the air (in case of wireless transmissions) such as MAC address or Wi-Fi SSID, can implement security flaws which can lead to guessing the credentials if there is a generation pattern based on these mentioned parameters. 

### Provision 1.3 

**Cryptography used for the authentication process should be from the best at the time market practice standards and appropriate to the properties of the technology, risk and usage.** 

### Provision 1.4 

**The change of authentication parameter should be able to be changed after setting up with an easy and simple process for the user and the administrator.** 

> Example 1:  For bio metric authentication values the device manufacturer allows this change in authentication value through retraining against a new bio metric. 

> Example 2: A parent in a household creates an account on the device for their child and selects and manages the PIN or password that the child uses. The parent is an administrator on the device and can restrict the child from changing the PIN or password. 

> Example 3: To make it simple for the user to change a password, the manufacturer designs the password change process in a way that, it requires a minimal number of steps. The manufacturer explains the process in a user manual and in a video tutorial. 

An authentication mechanism used for authenticating users, whether it be a fingerprint, password or other token, needs to have its value changeable. This is easier when this mechanism is part of the normal usage flow of the device. 

### Provision 1.5 

**A security implementation and basic mechanism of the device should be in such a way that brute force attacks become impractical if the device is not a constrained device.**

> Example 1: A device has a limitation on the number of authentication attempts within a certain time interval. It also uses increasing time intervals between attempts. 

> Example 2: The client application can lock an account or delay additional authentication attempts after a limited number of failed authentication attempts. 

This provision makes sure attacks like “credential stuffing” (doing a large-scale automated generation of login request based on a large list of possible credentials from a data breach or dictionary generation). And “exhausting the entire key-space” (brute forcing all the possible cryptographic keys of an algorithm) are a thing of the past.  

And attacks like the two mentioned and the similar ones should be detected and defended by the device while avoiding `resource exhaustion` and `denial of service`.

## Let's Connect

I welcome your insights, feedback, and opportunities for collaboration. Together, we can make the digital world safer, one challenge at a time.

- **LinkedIn**: (https://www.linkedin.com/in/aashwadhaama/)

I look forward to connecting with fellow cybersecurity enthusiasts and professionals to share knowledge and work together towards a more secure digital environment.
