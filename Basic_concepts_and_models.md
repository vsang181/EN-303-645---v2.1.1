# Basic concepts and models

## Architecture

A consumer IoT device comprises hardware and software components, typically with both physical and network interfaces. Figure illustrates a general example as well as a more complex "Smart Speaker" example. These architectural diagrams are illustrative, and it's not necessary for a device to have all or any of the depicted components.

![image](https://github.com/vsang181/ETSI-EN-303-645-V2.1.1-2020-06/assets/28651683/f2c74d3a-8688-44d8-a319-363d1d623e06)

In home deployments, consumer IoT setups typically include a mix of both constrained and non-constrained devices. These devices are often connected to the local area network (LAN), either directly through IP connectivity like Ethernet or Wi-Fi, or indirectly via a gateway or hub using non-IP connectivity protocols such as those based on [IEEE 802.15.4](https://standards.ieee.org/ieee/802.15.4/7029/). A router then links the LAN to the wide area network (WAN), which is typically the Internet. However, some devices within the home may connect directly to the WAN using other types of connections, whether IP or non-IP, such as GSM or LoRaWAN.

Consumer IoT devices in the home often connect to external online or local services. In this document, services provided by the manufacturer (such as telemetry or a companion mobile application) or those that are installed during initialization are classified as associated services. If the user chooses to install a service or access external content, it would not be considered an associated service.

For instance:

- Websites accessed via a device's browser are typically not considered associated services since the user decides to access them, not the device developer.

- Software applications (e.g., an "app" installed on a Smart TV) that come pre-installed are generally classified as associated services. However, if they are installed by the user through a store, they would not be associated.
 
- Connecting to a telemetry platform would be an associated service because it is usually pre-configured by the device manufacturer.

The figure bellow provides an example of an architecture for this model of deployment. The "home" boundary represents the approximate extent of the scope defined for the present document - including communication to associated services.

![image](https://github.com/vsang181/ETSI-EN-303-645-V2.1.1-2020-06/assets/28651683/bd5bf2a6-4bee-4a24-85c9-d0c441e318ea)

In the depicted setup in figure bellow, the following use cases clarify what would and would not be covered under the given definitions:

- Smart TV: The Smart TV communicates with two external services. The first is the Device Telemetry Service, which captures information from the TV with user permission for software improvement purposes. The second service is a Video Sharing Service accessed through a user-installed application, enabling entertainment streaming. The streaming service would not be considered an associated service.

- Gateway: The Gateway provides access to various constrained devices, including an IEEE 802.15.4 mesh network and a Light Sensor for home monitoring. It connects to a Cloud Access Service that allows remote control of the Smart Lock and sensor data viewing. This Cloud Access Service is an associated service.

- Smart Fridge: Equipped with a web browser, the Smart Fridge enables users to view news website headlines nearby. The news website would not be classified as an associated service.

- Weather Sensor: Used to monitor outdoor temperature, the Weather Sensor communicates via GSM directly to the WAN. The service it connects to for transmitting data is considered an associated service.

![image](https://github.com/vsang181/ETSI-EN-303-645-V2.1.1-2020-06/assets/28651683/fb1211c6-e909-44ad-8b95-b0fb5e9cebed)

## Device States

The present document does not cover the decommissioning of devices. A decommissioned device is one where sensitive data is not present. From manufacturing to decommissioning, a device transitions through several states, as illustrated in Figure A.4. In this model, a decommissioned device would be in the Factory Default state, as the Factory Reset process is typically used to remove all user data and configuration.

> Example: When decommissioned, a device can be recycled, resold or destroyed.

![image](https://github.com/vsang181/ETSI-EN-303-645-V2.1.1-2020-06/assets/28651683/f22110b8-99c3-4e1b-a886-bc69014ea1fe)

The next figure illustrates an example model of the data stored within an arbitrary device across different states. It's important to note that this model may vary depending on the specific device and scenario, and it's not expected to be identical for every case.

![image](https://github.com/vsang181/ETSI-EN-303-645-V2.1.1-2020-06/assets/28651683/9346570b-5dd3-45f5-af28-499dd8c14539)

## Let's Connect

I welcome your insights, feedback, and opportunities for collaboration. Together, we can make the digital world safer, one challenge at a time.

- **LinkedIn**: (https://www.linkedin.com/in/aashwadhaama/)

I look forward to connecting with fellow cybersecurity enthusiasts and professionals to share knowledge and work together towards a more secure digital environment.
