# 7. Ensure Software Integrity 

## Provision 7.1 

**The consumer IoT device should verify its software using secure boot mechanisms.** 

A hardware root of trust serves as a cornerstone in establishing strong attestation within a secure boot process. It acts as the foundation from which all other components in the system derive their trust, providing the source of cryptographic trust. This hardware component must be reliable and resistant to both physical and logical tampering since there's no way to detect if it's been compromised. By leveraging a hardware root of trust, a device can trust the results of cryptographic functions, such as those used in secure boot. This hardware root of trust can be supported by secure storage mechanisms for credentials or other alternatives that offer baseline security assurance tailored to the device's required security level. 

## Provision 7.2 

**If an unauthorized change is detected to the software, the device should alert the user and/or administrator to the issue and should not connect to wider networks than those necessary to perform the alerting Function.** 

Remote recovery from unauthorized changes can depend on having a known safe state, like storing a verified version locally for secure recovery and updates. This prevents service disruptions and costly recalls or maintenance, while also managing the risk of device takeover by attackers manipulating update or network communication methods. 

If a consumer IoT device detects unauthorized software changes, it can alert the appropriate stakeholders. Additionally, some devices can enter an administration mode for management purposes. 

> Example: A thermostat in a room can have a user mode; this mode prevents changing of other settings. If an unauthorized software change is detected, an alert to the administrator is appropriate, as the administrator can act on the alert (whereas a user does not). 

>  An attack that forces a device to revert to a known good state can introduce a DoS risk if the device is unable to successfully perform this or if the attacker is able to repeatedly cause this effect.

## Let's Connect

I welcome your insights, feedback, and opportunities for collaboration. Together, we can make the digital world safer, one challenge at a time.

- **LinkedIn**: (https://www.linkedin.com/in/aashwadhaama/)

I look forward to connecting with fellow cybersecurity enthusiasts and professionals to share knowledge and work together towards a more secure digital environment.
