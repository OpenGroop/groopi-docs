# Network Guide

## Introduction
OpenGro/Op's ability to operate on a network is a big deal. This means that we can access OpenGro/Op over many different network topologies, whether private, local, public/remote, or pushing data to the cloud. This makes OpenGro/Op/RPi combo very flexible. However, it must be noted that this flexibilty does require, if anything, a basic knowledge of how networks work.  

OpenGro/Op is accessed using a web browser on a device that shares it's network with the RPi. Following the [Quickstart Guide](/opengroop-quickstart/) shows us one way of sharing a network with the RPi. In this case, the RPi functions as a WIFI Access Point (AP), just like a WIFI router, inviting other devices to join it's network, given the proper credentials. Devices that join the RPi's network now share it's network and can now access OpenGro/Op.  

Another way to have devices share a network with the RPi is to connect the RPi to a router which shares connections with other devices already. This is defined as a local network. Any device with a web browser connected to the router (local network) will be able to access OpenGro/Op. The RPi itself can connect to local networks via WIFI or ethernet.  





## Local Server connection


The Raspberry Pi can connect to local networks via 2 methods, ethernet or WIFI.

#### Connect RPi via Ethernet to networks

Connecting your RPi to a local network via ethernet is the simplest way to connect to a network.
It requires no configuration, as long as your router is configured to hand out IP addresses automatically (DHCP).  

These steps assume that your browsing device is connected to the RPi's WIFI ACCESS POINT and have taken necessary steps to log in.

1. Connect an ethernet cable between the RPi and your router.
2. Go to ***Settings / NETWORK / LOCAL NETWORK***.
3. Take note of the IP address in the ***ETHERNET INTERFACE*** section.
4. Any device connected to the router can now access OpenGro/Op using the above noted IP address.  



The RPi gateway server topology

```
        REMOTE NETWORK               LOCAL NETWORK                     ACCESS POINT
            IP ADDRESS *              IP ADDRESSES *                 * IP ADDRESS
                       |                           |                 |
               +---+   |   +--------+              |   +---------+   |
               | I |   |   |        |              |   |         |   |
+--------+     | N |   |   |        |               \  | RPi     |   |
| Phone  |     | T |    \  |        | <= Ethernet => * | Gateway |  /           +---------+
| Tablet | <=> | E | <=> * | Modem/ |                | | Server  | * <= WIFI => | Phone   |
| etc..  |     | R |       | Router | <= WIFI =====> * |         |              | Tablet  |
+--------+     | N |       |        |                  +---------+              | Desktop |
               | E |       |        | <= WIFI/Ethernet =======================> | etc.... |
               | T |       |        |                                           +---------+
               +---+       +--------+

          |___|     |_____|          |________________|           |____________|
            |          |                     |                           |
Remote -----+          |                     |                           |
WAN    ----------------+                     |                           |
Local Network -------------------------------+                           |
Access Point  -----------------------------------------------------------+

```
