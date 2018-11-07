# Connecting the Raspberry Pi Gateway Server to a router

The Raspberry Pi (RPi) gateway server can connect to a router and have the OpenGro/Op web app be available over the router's network. Any device connected to the router can access the OpenGro/Op web app.  

## Requirements
- A router. It can be a WIFi and/or Ethernet router.  
- The router must be configured to hand out IP addresses automatically (DHCP).  
  If you have not configured the router otherwise, then don't worry about this.

## Network Interfaces

The RPi has two network interfaces to connect with routers:

- Ethernet Interface
- WIFI Interface

When connected to a router, each of these interfaces will be issued an IP address by the router. The IP addresses issued to the interfaces will be the IP addresses used to access OpenGro/Op on the network. Because the router issues these IP addresses automatically, we have no way of knowing beforehand what the  IP address will be. For this reason, we'll need access to the OpenGro/Op web app while connected to the RPi's WIFI Access Point *(as we did in the [Quickstart Guide](/opengroop-quickstart/))*.  


### Connect the Rasbperry Pi to a Router via it's Ethernet interface
While your browsing device is connect to the RPi's WIFI Access Point (AP):

1. Point your web browser to http://10.10.10.1.
2. Log in to OpenGro/Op as *'admin'*.
3. Go to ***Settings -> NETWORK -> LOCAL NETWORK***  
  *(the Ethernet interface IP address will be listed *'(not connected)'*)*
4. Connect an Ethernet cable between the router and the RPi.
5. Wait a few seconds (20s should do..), then refresh the page. There should now be an IP addressed associated with the Ethernet interface. Take note of this IP address. It will be the IP address used to access OpenGro/Op over the network.
6. Log out of OpenGro/Op
7. Connect your browsing device to the router and point it's web browser to the Ethernet interface's IP address. Log in.. and profit.

### Connect the Raspberry Pi to a WIFI Router
To connect the RPi to a WIFI router's network, we need access to the OpenGro/Op web app. We need to have an established connection with the RPi, either via it's WIFI Access Point or ethernet interface, to configure the WIFI network settings.  
When configuring the RPi gateway server's to connect to a WIFI network, I recomend establishing an ethernet connection with the router first *(see section above)*, then accessing OpenGro/Op over the local network.    

If it is impossible or inconceivable to connect the RPi to the router via ethernet, jump to the next section *(Connecting the Raspberry Pi to a WIFI Router via the Access Point)*.

While our RPi gateway server is connected to the router via it's ethernet interface:

1. Point your web browser to the RPi's ethernet interface IP address.
2. Log in to OpenGro/Op as *'admin'*.
3. Got to ***Settings -> NETWORK -> LOCAL NETWORK***  
  You'll notice the WIFI interface IP address is listed as *'(not connected)'*
4. Click ***configure***.
5. Select the WIFI network you would like to join.
6. Enter the password, then click ***SUBMIT***.
7. You'll be redirected back to the local network settings page. There should now be an IP address associated with the WIFI interface.  
  Take not of this IP address. It will be the IP address used to access OpenGro/Op over the network's WIFI.  
  If the IP address is still listed as *'(not connected)'*, then the password was incorrect. Repeat steps 4 to 6 until a connection has been established.
8. Once a connection is established and you have noted the WIFI interface's IP address, log out of OpenGro/Op.
9. Disconnect the ethernet connection between the RPi and the router
10. Point your web browser to the WIFI interface's IP address, log in, and profit!!

#### Connecting the Raspberry Pi to a WIFI Router via it's Access Point.

Although the RPi has 2 seperate WIFI interfaces *(WIFI Access Point and local WIFI interface)*, they both share the same antennea. While configuring the local WIFI settings for the RPi, the RPi needs to reset the antenna. This forces the Access Point connection to drop.

1. Point your web browser to 10.10.10.1.
2. Log in to the OpenGro/Op web app as *'admin'*.
3. Got to ***Settings -> NETWORK -> LOCAL NETWORK***  
  You'll notice the WIFI interface IP address is listed as *'(not connected)'*
4. Click ***configure***.
5. Select the WIFI network you would like to join.
6.
