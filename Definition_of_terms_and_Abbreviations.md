# Definition of terms and Abbreviations 

## Terms 

- **Administrator**: a user with the highest possible privilege for any user of a device, which translates to the ability to change any configuration related to intended functionality. 

- **associated service**: a digital service that works in partnership with the device making its combined experience the overall IoT product and these services are typically required to provide the product’s intended functionality. 

> Example 1: Associated services can include mobile applications, cloud computing/storage and third-party Application Programming Interfaces (APIs). 

> Example 2: A device transmits telemetry data to a third-party service chosen by the device manufacturer. This service is an associated service. 

- **authentication mechanism**: A method used to identify the authentify of an entity. 

> An `entity` can either be a user or a machine. 

> Example: An authentication mechanism can be the requesting of a password, scanning a QR code, or use of a biometric fingerprint scanner. 

- **authentication value**: an Individual value utilized by an authentication mechanismas an attribute. 

> Example: When the authentication mechanism is to request a password, the authentication value can be a character string. When the authentication mechanism is a biometric fingerprint recognition, the authentication value can be the index fingerprint of the left hand. 

- **best practice cryptography**: Use of right type and form of cryptography depending on the particular use case scenario and the one with no possibility of an attack based on the readily available techniques on the market. 

> This does not refer only to the cryptographic primitives used, but also implementation, key generation and handling of keys. 

> Multiple organizations, such as SDOs and public authorities, maintain guides and catalogues of cryptographic methods that can be used. 

> Example: The device manufacturer uses a communication protocol and cryptographic library provided with the IoT platform and where that library and protocol have been assessed against feasible attacks, such as replay. 

- **constrained device**: Devices that by design have restricted storage, processing. Communication and interacting capabilities and execute their tasks with minimal power input stay cost-effective. 

> Physical limitations can be due to power supply, battery life, processing power, physical access, limited functionality, limited memory or limited network bandwidth. These limitations can require a constrained device to be supported by another device, such as a base station or companion device. 

> Example 1: A window sensor's battery cannot be charged or changed by the user; this is a constrained device. 

> Example 2: The device cannot have its software updated due to storage limitations, resulting in hardware replacement or network isolation being the only options to manage a security vulnerability. 

> Example 3: A low-powered device uses a battery to enable it to be deployed in a range of locations. Performing high power cryptographic operations would quickly reduce the battery life, so it relies on a base station or hub to perform validations on updates. 

> Example 4: The device has no display screen to validate binding codes for Bluetooth pairing. 

> Example 5: The device has no ability to input, such as via a keyboard, authentication information. 

> A device that has a wired power supply and can support IP-based protocols and the cryptographic primitives used by those protocols is not constrained. 

> Example 6: A device is mains powered and communicates primarily using TLS (Transport Layer Security).

- **consumer**: a person who purchases goods and services for personal use.

> Organizations, including businesses of any size, use consumer IoT. For example, Smart TVs are frequently deployed in meeting rooms, and home security kits can protect the premises of small businesses.

- **consumer IoT device**: A network connected or network connectable device that having the ability to connect with associated services. Used by consumers at home or as electronic wearables.

> Consumer IoT devices are commonly also used in business contexts. These devices remain classified as consumer IoT devices.

> Consumer IoT devices are often available for the consumer to purchase in retail environments. Consumer IoT devices can also be commissioned and/or installed professionally.

- **critical security parameter**: Information related to security which can compromise security in multiple ways if disclosed.

> Example: Secret cryptographic keys, authentication values such as passwords, PINs, private components of certificates.

- **debug interface**: Not a consumer facing functionality but a physical interface for the manufacturer to communicate with the device during development or to perform triage of issues.

> Example: Test points, UART, SWD, JTAG.

- **defined support period**: Minimum period for which the manufacturer will provide security updates.

> This definition focuses on security aspects and not other aspects related to product support such as warranty.

- **device manufacturer**: Entity that creates the final consumer IoT product, may contain products and components of other entities.

- **factory default**: State of the device after factory reset or after final production assembly.
 
> This includes the physical device and software (including firmware) that is present on it after assembly.

- **initialization**: It can be defines as the operation that involves activating the network connectivity of the device and sometimes sets authentication features for network access.

- **initialized state**: State of the device after initialization.

- **IoT product**: Consumer IoT device and its associated services.

- **isolable**: It is the ability to be isolated from a network while being connected to it, considering the functionality loss is not related to its main function but the additional functionalities that came with the connectivity.

> A Smart Fridge has a touchscreen-based interface that is network-connected. This interface can be removed without stopping the fridge from keeping the contents chilled.  

- **logical interface**: Software implementation that utilizes a network interface to communicate over the network via channels or ports.
 
- **manufacturer**: Relevant economic operator in the supply chain (including the device manufacturer).

> This definition acknowledges the variety of actors involved in the consumer IoT ecosystem and the complex ways by which they can share responsibilities. Beyond the device manufacturer, such entities can also be, for example and depending on a specific case at hand: importers, distributors, integrators, component and platform providers, software providers, IT and telecommunications service providers, managed service providers and providers of associated services.

- **network interface**: Physical interface that can be used to access the functionality of consumer IoT via a network.
 
- **owner**: User who owns or who purchased the device.
 
- **personal data**: Any information relating to an identified or identifiable natural person.

> This term is used to align with well-known terminology but has no legal meaning within the present standard's documentation.

- **physical interface**: Physical port or air interface (such as radio, audio or optical) used to communicate with the device at the physical layer.

> Radios, ethernet ports, serial interfaces such as USB, and those used for debugging.

- **public security parameter**: Public information whose modification can compromise the security.

> Example 1: A public key to verify the authenticity/integrity of software updates.

> Example 2: Public components of certificates.

- **remotely accessible**: Intended to be accessible from outside the local network.

- **security module**: Set of hardware, software, and/or firmware that implements security functions.

> Example: A device contains a hardware root of trust, a cryptographic software library that operates within a trusted execution environment, and software within the operating system that enforces security such as user separation and the update mechanism. These all make up the security module.

- **security update**: Software update issued by the manufacturer to issue discovered vulnerabilities.

> Software updates can be purely security updates if the severity of the vulnerability requires a higher priority fix.

- **sensitive security parameters**: Critical and public security parameters.

- **software service**: Software component used to support the functionality of a device.

> Example:  A runtime for the programming language used within the device software or a daemon that exposes an API used by the device software, e.g. a cryptographic module's API.

- **telementry**: Identifying information for the manufacturer used to identify issues or information related to device usage.

> Example: A consumer IoT device reports software malfunctions to the manufacturer enabling them to identify and remedy the cause.

- **unique per device**: Unique for each individual device of a given product class or type.

- **user**: Person or organization using the device or service.

## Abbreviations

|Abbreviation|Description|
|---|---|
|API|Application Programming Interface|
|ASLR|Address Space Layout Randomization|
|CVD|Coordinated Vulnerability Disclosure|
|CVRF|Common Vulnerability Reporting Framework|
|DDoS|Distributed Denial of Service|
|DSC|Dedicated Security Components|
|ENISA|European Union Agency for Network and Information Security|
|GDPR|General Data Protection Regulation|
|GSM|Global System for Mobile communications|
|GSMA|GSM Association|
|IEEE|Institute of Electrical and Electronics Engineers|
|IoT|Internet of Things|
|IP|Internet Protocol|
|ISO|International Organization for Standardization|
|JTAG|Joint Test Action Group|
|LAN|Local Area Network|
|LoRaWAN|Long Range Wide Area Network|
|MAC|Media Access Control|
|NIST|National Institute of Standards and Technology|
|NX|No execute|
|OTP|One-Time Password|
|QR|Quick Response|
|SBOM|Software Bill of Materials|
|SDO|Standards Development Organization|
|SE|Secure Elements|
|SSID|Service Set IDentifier|
|STRIDE|Spoofing, Tampering, Repudiation, Information disclosure, Denial of service, Elevation of privilege|
|SWD|Serial Wire Debug|
|TEE|Trusted Execution Environment|
|TS|Technical Specification|
|UART|Universal Asynchronous Receiver-Transmitter| 
|UI|User Interface|
|USB|Universal Serial Bus|
|WAN|Wide Area Network|

## Let's Connect

I welcome your insights, feedback, and opportunities for collaboration. Together, we can make the digital world safer, one challenge at a time.

- **LinkedIn**: (https://www.linkedin.com/in/aashwadhaama/)

I look forward to connecting with fellow cybersecurity enthusiasts and professionals to share knowledge and work together towards a more secure digital environment.
