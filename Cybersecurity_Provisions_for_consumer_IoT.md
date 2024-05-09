# Cybersecurity Provisions for consumer IoT 

For simplifying our understanding, we will not use the provision’s numbering from the official documentation but use the term “Provision 1”, “Provision 2”, “Provision 3” and so on instead of “Provision 5”  

## 1 No universal default passwords 

### Provision 1.1  

Where passwords are used and, in any state, other than the factory default, all consumer IoT device passwords shall be unique per device or defined by the user. 

> Multiple ways can be used to perform authentication and authentication is not limited to passwords. But when the passwords are used [NIST Special Publication 800-63B](https://pages.nist.gov/800-63-3/sp800-63b.html) 

As a majority of IoT devices in the markets come with default credentials (such as “admin”:”admin”). Which have led to multiple accounts of security incidents. And this practice of default credentials has an absolute need to be discontinued. It can be remediated by using giving default pre-install credentials which are completely unique per device or by forcing the user/entity to change them before being able to use any functionality of the device or maybe using password independent methods. 

> Example: During initialization a device generates certificates that are used to authenticate a user to the device via an associated service like a mobile application. 

A multi factor authentication method could be used for better security implementation. 

### Provision 1.2 

This is a provision where pre-initialized credentials are used and these should be generated with a mechanism that reduces the risk of automated attacks against a class or type of device. 

> Example: Pre-installed credentials are sufficiently randomized. 

A pattern of passwords like “Password1”, “Password2”, “Password3” are easily recognizable. Also parameters sent over the same network or over the air (in case of wireless transmissions) such as MAC address or Wi-Fi SSID, can implement security flaws which can lead to guessing the credentials if there is a generation pattern based on these mentioned parameters. 

### Provision 1.3 

Cryptography used for the authentication process should be from the best at the time market practice standards and appropriate to the properties of the technology, risk and usage. 

### Provision 1.4 

The change of authentication parameter should be able to be changed after setting up with an easy and simple process for the user and the administrator. 

> Example 1:  For bio metric authentication values the device manufacturer allows this change in authentication value through retraining against a new bio metric. 

> Example 2: A parent in a household creates an account on the device for their child and selects and manages the PIN or password that the child uses. The parent is an administrator on the device and can restrict the child from changing the PIN or password. 

> Example 3: To make it simple for the user to change a password, the manufacturer designs the password change process in a way that, it requires a minimal number of steps. The manufacturer explains the process in a user manual and in a video tutorial. 

An authentication mechanism used for authenticating users, whether it be a fingerprint, password or other token, needs to have its value changeable. This is easier when this mechanism is part of the normal usage flow of the device. 

### Provision 1.5 

A security implementation and basic mechanism of the device should be in such a way that brute force attacks become impractical if the device is not a constrained device. 

> Example 1: A device has a limitation on the number of authentication attempts within a certain time interval. It also uses increasing time intervals between attempts. 

> Example 2: The client application can lock an account or delay additional authentication attempts after a limited number of failed authentication attempts. 

This provision makes sure attacks like “credential stuffing” (doing a large-scale automated generation of login request based on a large list of possible credentials from a data breach or dictionary generation). And “exhausting the entire key-space” (brute forcing all the possible cryptographic keys of an algorithm) are a thing of the past.  

And attacks like the two mentioned and the similar ones should be detected and defended by the device while avoiding `resource exhaustion` and `denial of service`. 

## 2 Implement a means to manage reports of vulnerabilities 

### Provision 2.1 

There should be a vulnerability disclosure policy available publicly. With keeping the following points in mind while writing the policy- 

• Contain information on how to report issues. 

• Information on timelines for: 

1. Initial acknowledgement of receipt 

2. Status updates until the resolution of the reported issues. 

This policy is a well-defined set of rules for security researchers and anyone who wants to report any issues. The policy should be updated whenever necessary to show more transparency and clarity on the dealing of the manufacturer’s behavior to such issues. 

`Coordinated Vulnerability Disclosure` (CVD) is a set of processes defined on how to deal with disclosures about potential security vulnerabilities and to support the remediation of such. CVD is standardized by ISO in [ISO/IEC 29147](https://drive.google.com/file/d/1OGSTLcfY7fA20WZAEdvgnUIGqtpoFBhi/view?usp=sharing)  For disclosing vulnerabilities and have been proved successful over time. 

> CVD is not a common thing for the current IoT industry as many of the companies still do not understand how to properly deal with security researchers finding vulnerability in their products/devices. 

### Provision 2.2 

All the vulnerabilities disclosed should be acted on in a timely manner. 

The time-span to act on a discovered vulnerabilities can vary on multiple factors and are always incident specific. However, in general case scenarios it is supposed to be done in 90 days (about 3 months) for a software solution, including availability of patches and notification of the issue. Meanwhile a hardware fix can take longer considering the situation. 

### Provision 2.3 

For the defined support period, manufacturers should continuously monitor, identify and rectify their security vulnerabilities for the devices and services they offer or have offered in the past.

> Manufacturers are expected to exercise due care for all software and hardware components used in the product, this includes due care related to the selected third parties that provide associated services to support the functions of the product.

Vulnerabilities are expected to be reported directly to the affected stakeholders in the first instance. If that is not possible, vulnerabilities can be reported to national authorities. Manufacturers are also encouraged to share informationwith competent industry bodies, such as the GSMA and the IoT Security Foundation. Guidance on Coordinated Vulnerability Disclosure is available from the IoT Security Foundation which references [ISO/IEC 29147](https://drive.google.com/file/d/1OGSTLcfY7fA20WZAEdvgnUIGqtpoFBhi/view?usp=sharing).

Manufacturers that provide IoT products have a duty of care to consumers and third parties who can be harmed by their failure to have a CVD programme in place.
 
Disclosures can comprise different approaches depending on the circumstances:

- Vulnerabilities related to single products or services: the problem is expected to be reported directly to the affected stakeholder (usually the device manufacturer, IoT service provider or mobile application developer). The source of these reports can be security researchers or industry peers.

- Systemic vulnerabilities: a stakeholder, such as a device manufacturer, can discover a problem that is potentially systemic. Whilst fixing it in the device manufacturer's own product is crucial, there is significant benefit to industry and consumers from sharing this information.

> The Common Vulnerability Reporting Framework ([CVRF](http://docs.oasis-open.org/csaf/csaf-cvrf/v1.2/csaf-cvrf-v1.2.html)) can also be useful to exchange
information on security vulnerabilities.

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 



