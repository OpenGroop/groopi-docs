# OpenGro/Op Quickstart Guide v0.2.9
This quickstart guide will guide you through the process of getting your OpenGro/Op system up and running quickly. But before we start, let's get familiar our setup.

## What's included

### Hardware
- 1 temperature/humidity/photocell sensor (STHP) with a 15' lead to a USB male connector
- 1 Raspberry Pi (RPi) gateway server
- AC/DC power supply for RPi

### Software
- OpenGro/Op web app - *used to interface with the server*


## Requirements

- A WIFI cabable device with a web browser. This can be on a phone, tablet, laptop, etc.., anything with a web browser.
- Javascript and cookies must be enabled on the browser. If you haven't explicitly disabled these, then they are most likely already enabled.
- A printed or downloaded [PDF](https://git.opengroop.org/groopi-quickstart-v0.2.6.pdf) version of this guide.  
(This is only necessary if you plan on following this guide on the same device that you plan to connect to the RPi server gateway.)

## Step Summary

To get us up and going, these are the steps we will be taking:

1. Placing the RPi and sensor in a suitable location.
2. Powering up the RPi.
3. Connecting your browsing device to the RPi's WIFI network.
4. Browse to the OpenGro/Op web app and login.
5. Connecting the sensor to the RPi.
6. Changing the default password for the OpenGro/Op web app.  


## Placing the RPi and sensor in a suitable location.
The STHP sensor is equipped with a 15' lead cable which connects to the RPi gateway via USB. When deciding where to place these, there are some considerations that should be made.

#### STHP considerations
The STHP (as well as most other temp/humidity sensor;) will give a biased reading when place in areas that have high wind activity. While air movement is good for readings, placing the STHP directly in the path of fans (either in front, or behind) is discouraged.

#### RPi gateway server considerations
The RPi gateway server runs a wireless access point which we use to connect to it. This is just like any typical WIFI network we connect to. Because of this, it should not be placed anywhere that impedes it's signal.   

## Power up the RPi

1. Leave the sensor disconnected.
2. Connect the micro USB end of the AC/DC power supply to the RPi.
4. Plug the plug end of the AC/DC power supply into a 120v power source.  

Your RPi should now power up with the LED indicators signaling so. After a few seconds (about 20s), the LED indicators will stop flashing and go dark. Although normal, the RPi is not fully booted yet and will take a few more minutes to finish booting. We can't move on until fully booted. I suggest waiting 5 minutes before moving on to the next step.

## Next step

Did you wait 5 minutes? Don't cheat. Wait the full 5.  

## Connecting to the Groopi's WIFI network

With our 5 minutes up, let's continue.

You will be connecting to the RPi's WIFI network the same way you would connect to any other WIFI network. Your RPi's network name and password are labeled on the RPi.

1. With your browsing device (phone, tablet, etc..), search for the RPi's WIFI network (labeled on the RPi). This is usually done in your device's WIFI settings.
2. Select the RPi's WIFI network.
3. Enter the RPi's WIFI network password when prompted.

You should now be connected to the RPi's WIFI network. Now you're ready to access the OpenGro/Op web app.

> ***Note:*** *While connected to the RPi's WIFI connection, your browsing device will not have Internet access through it's WIFI connection.*

## Browse to the OpenGro/Op web app

With your browsing device connected to the RPi's WIFI network, open up a browser and enter this IP address into the address bar:

- 10.10.10.1

This will take you to the OpenGr/Op web app login page.  

#### Log in to access the OpenGro/Op web app

The login credentials are:  

- USERNAME: ***admin***
- PASSWORD: ***opengroop***


After a successful login, you'll be directed to the *Sensors* section. This is where your sensors will be listed, showing their current readings.  

## Connecting the sensor

You can now connect the STHP sensor to any of the RPi's USB ports. Once connected, refresh the *Sensors* page and the sensor will be listed.  
It will initially display a zero reading. After 60 seconds, current readings will be available by refreshing the page. Readings are updated in 60 second intervals and can be viewed by refreshing the page.  

#### View sensor data
Selecting the sensor will direct you to the sensor's chart page where you can view charts based on the sensor's data. Refreshing this page will also update the current reading.  
Selcting *SENSOR SETTINGS*,  will give you access to the STHP's settings, such as format (Celsius or Fahrenheit) and alias.

> ***Note:*** *While current readings will be immediately stored and available for viewing, charts will be initially delayed. Hourly charts will appear after 30 minutes. Daily summary charts will appear in 2 days. This delay will occur only once, the first time a sensor is connected to the RPi.*

## Change default password for the OpenGro/Op web app (*optional*)

Although not required, it is strongly advised that you change the default *'admin'* user password.  

1. On the main navigation, select *SETTINGS*
2. Select *USERS*
3. In the *EDIT USER* section, select the user *'admin'* (it will be the only user available)
4. Enter the new password twice, then *SUBMIT*.

#### Note on changing the *admin* password

There are currently no facilities to reset this password if forgotten. So please **do not outsmart yourself by picking a complicated password**. The objective here is to change the password from the default one provided, which is a publicly known password.

## That's it!

Whenever you want to view your sensor's data, just join the RPi's WIFI network, browse to the OpenGro/Op web app (10.10.10.1), and log in. Just remember that your browsing device will not have Internet access through it's WIFI while connected to the RPi's WIFI network.  

## Is that really it?

Absolutely not. Check out the [User Guides](/opengroop-guides/) to see what OpenGro/Op can do.  
