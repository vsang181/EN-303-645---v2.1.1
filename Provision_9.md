# 9. Make System Resilient to Outages 

The goal of this provision is to guarantee the continuous operation of IoT services, especially as consumers integrate IoT devices into various aspects of their lives, including safety-critical functions. While safety-related regulations may be applicable, the focus is on preventing outages from negatively affecting users and designing products and services with resilience to these challenges. 

## Provision 9.1 

**Resilience should be built into consumer IoT devices and services, taking into account the possibility of outages of data networks and power.** 

## Provision 9.2 

**Consumer IoT devices should remain operating and locally functional in the case of a loss of network access and should recover cleanly in the case of restoration of a loss of power.** 

> "Recovering cleanly" normally involves resuming connectivity and functionality in the same or improved state. 

## Provision 9.3 

**The consumer IoT device should connect to networks in an expected, operational and stable state and in an orderly fashion, taking the capability of the infrastructure into consideration.** 

> Example 1: A Smart Home loses connection to the internet following a power outage. When the network connection is restored, the devices in the home reconnect after a randomized delay to minimize network utilization. 

> Example 2: After making an update available, the manufacturer notifies devices in batches to prevent them all simultaneously downloading the update. 

As IoT systems and devices become increasingly vital for consumers, especially in safety-critical or life-impacting scenarios, it's essential to ensure their reliability. One way to enhance resilience is by maintaining local service operation in case of network loss. Additionally, incorporating redundancy into associated services and implementing measures to mitigate Distributed Denial of Service (DDoS) attacks or signaling storms—caused by mass reconnections of devices after an outage—can bolster resilience. The necessary level of resilience should be proportional to the device's usage, considering the impact on others who rely on the system, service, or device, as an outage can have broader consequences than anticipated. 

Orderly reconnection refers to reconnecting devices in a way that prevents a sudden influx of simultaneous requests, like for software updates or reconnections, from numerous IoT devices. This involves taking deliberate measures, such as introducing a random delay before attempting to reconnect, following an incremental back-off mechanism.

## Let's Connect

I welcome your insights, feedback, and opportunities for collaboration. Together, we can make the digital world safer, one challenge at a time.

- **LinkedIn**: (https://www.linkedin.com/in/aashwadhaama/)

I look forward to connecting with fellow cybersecurity enthusiasts and professionals to share knowledge and work together towards a more secure digital environment.
