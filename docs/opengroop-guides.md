# OpenGro/Op User Guides

[Quickstart Guide](//)  
[Network Guide](//)  
[Cloud Gateway Server Guide](//)  
[OpenGro/Op Reference Guide](//)  

OpenGro/Op is a web application, designed to run on a server, in this case a [Raspberry Pi](/wikipedia_page/) (RPi), over a network.   

The RPi's network design allows it to operate at 3 successive levels:

1. Private Server  
  *(connecting to the RPi directly through it's WIFI access point; only those connected to the RPi can access the OpenGro/Op web app)*  

2. Local / Public Server  
  *(connecting the RPi to a router and accessing the OpenGro/Op web app over that router's network; this also can make the OpenGro/Op web app available over the Internet if the router has an Internet connection)*  

3. Cloud Gateway Server  
  *(OpenGro/Op will push all sensor data to the cloud, to be made available to any device with an Internet connection)*  

#### Private Server
Out of the box, the RPi functions as private server. If this is all you require, then you're good to go. Just connect to the RPi's WIFI access point and browse 10.10.10.1 to access OpenGro/Op.  

Accessing OpenGro/Op privately is covered in the [Quickstart Guide](//).

#### Local / Public Server
If, though, you do not want to have to switch networks to access the OpenGro/Op web app,
the RPi can connect to your existing local network (WIFI or ethernet) making OpenGro/Op available on the local network *(local server)*. This also has the benefit of allowing the OpenGro/Op web app to be available remotely over the Internet *(public server)*, although doing so requires an Internet connection as well as every router between the RPi and the Internet to be configured to allow it.   

To configure OpenGro/Op to available as a local and/or public server, follow the [Network Guide](#local connections).  

#### Cloud Gateway Server
If having Internet access to your data is important, yet configuring routers is not possible or conceivable, OpenGro/Op can push your sensor data to the cloud. Your readings will be available to any device that has an Internet connection.  

To configure OpenGro/Op to push sensor data to the cloud, follow the [Cloud Gateway Server Guide](#cloud gateway).

#### OpenGro/Op Reference Guide  

Detailed web app reference is privided in the [OpenGro/Op Reference Guide](//)
