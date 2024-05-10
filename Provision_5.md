# 5. Communicate Securely 

## Provision 5.1 

**The consumer IoT device shall use best practice cryptography to communicate securely.** 

The effectiveness of security measures, like encryption, depends on various factors such as how the technology is used. Since security threats are always changing, it's hard to give fixed advice on cryptography or other security methods without it becoming outdated quickly. 

## Provision 5.2 

**The consumer IoT device should use reviewed or evaluated implementations to deliver network and security functionalities, particularly in the field of cryptography.** 

Reviews and evaluations can involve an independent internal or external entity. 

> Example: Distributed software libraries within the development and test community, certified software modules, and hardware equipment crypto-service providers (such as the Secure Element and Trust Execution Environment) are all reviewed or evaluated. 

## Provision 5.3 

**Cryptographic algorithms and primitives should be updateable.** 

> This is also known as “cryptoagility”. 

For devices that can't receive updates, it's crucial that the device's lifespan doesn't surpass the recommended usage lifespan of the cryptographic algorithms it relies on, including their key sizes. 

## Provision 5.4 

**Access to device functionality via a network interface in the initialized state should only be possible after authentication on that interface.** 

> Functionality can vary significantly on the use case and can encompass a range of things, including access to personal data and device actuators. 

Some devices, like those in the Web of Things, freely provide public data without needing authentication. However, these devices can still be vulnerable to attacks through their network services. Using a proper authentication method can help prevent unauthorized access and strengthen the device's overall security. Regarding configuration changes made over a network interface, they should only be accessible after authentication, except for cases where network service protocols essential for device operation require unauthenticated access due to uncertainty about required configurations. 

> Protocols that are an exception include ARP, DHCP, DNS, ICMP and NTP. 

> Example: Security-relevant changes include permission management, configuration of network keys and password changes. 

##Provision 5.6 

**Critical security parameters should be encrypted in transit, with such encryption appropriate to the properties of the technology, risk and usage.** 

 

## Provision 5.7 

**The consumer IoT device shall protect the confidentiality of critical security parameters that are communicated via remotely accessible network interfaces.** 

Various methods are available for enrollment and authentication, ranging from out-of-band mechanisms like QR codes to human-readable options like passwords. 

When authentication involves unique values for each attempt, like in challenge-response setups or one-time passwords, the response isn't the actual authentication value. Nonetheless, it's advisable to keep these values confidential. 

Confidentiality can be ensured through encrypted communication channels or payload encryption. Typically, protocols or algorithms as robust as the transmitted key material are used for this purpose, although other measures like requiring physical proximity can also be effective. 

## Provision 5.8  

**The manufacturer shall follow secure management processes for critical security parameters that relate to the device.** 

It's highly recommended to utilize open, peer-reviewed standards for critical security parameters, commonly known as "key management."

## Let's Connect

I welcome your insights, feedback, and opportunities for collaboration. Together, we can make the digital world safer, one challenge at a time.

- **LinkedIn**: (https://www.linkedin.com/in/aashwadhaama/)

I look forward to connecting with fellow cybersecurity enthusiasts and professionals to share knowledge and work together towards a more secure digital environment.
