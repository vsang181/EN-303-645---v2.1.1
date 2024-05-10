# 4. Securely Store Sensitive Security Parameters 

## Provision 4.1 

**Sensitive security parameters in persistent storage shall be stored securely by the device.** 

Secure storage methods can safeguard important security details. These methods can include Trusted Execution Environments (TEE), encrypted storage linked to the hardware, Secure Elements (SE) or Dedicated Security Components (DSC), and processing abilities of software on a UICC card. 

> This provision applies to persistent storage, but manufacturers can also implement similar approaches for sensitive security parameters in memory. 

> Example 1: The root keys involved in authorization and access to licensed radio frequencies (e.g. LTE-m cellular access) are stored in a UICC. 

> Example 2: A remote controlled door-lock using a Trusted Execution Environment (TEE) to store and access the sensitive security parameters. 

> Example 3: A wireless thermostat stores the credentials for the wireless network in a tamper protected microcontroller rather than in external flash storage. 

## Provision 4.2 

** Where a hard-coded unique per device identity is used in a device for security purposes, it shall be implemented in such a way that it resists tampering by means such as physical, electrical or software.** 

> Example: A master key used for network access that is unique to the device is stored in UICC which is compliant to relevant ETSI standards.  

## Provision 4.3 

**Hard-coded critical security parameters in device software source code shall not be used.** 

Reverse engineering of devices and apps can expose sensitive information like fixed usernames, passwords, or API keys. These keys can grant access to important functions in remote services, or private keys used for secure communication protocols. Typically, these credentials are stored directly in the source code, which is risky. Even basic attempts to hide or encrypt this information can be easily bypassed. 

## Provision 4.4 

**Any critical security parameters used for integrity and authenticity checks of software updates and for protection of communication with associated services in device software shall be unique per device and shall be produced with a mechanism that reduces the risk of automated attacks against classes of devices.** 

> Example 1: A different symmetric key is deployed on every device of the same product class for generating and verifying message authentication codes for software updates. 

> Example 2: The device uses the manufacturer's public key to verify a software update. This is not a critical security parameter and does not need to be unique per device. 

Equipping a device with unique and crucial security parameters safeguards the reliability and genuineness of software updates and the device's communication with related services. If common critical security parameters are employed, their exposure could lead to large-scale assaults on other IoT devices, potentially enabling the formation of botnets. 
