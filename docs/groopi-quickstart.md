# Groopi Quickstart Guide v0.2.6
This quickstart guide will guide you through the process of getting your Groopi up and running quickly. But before we start, there are few requirements.


## Requirements

1. A WIFI cabable device with a web browser. This can be on a phone, tablet, laptop, etc.., anything with a web browser.
2. Javascript and cookies must be enabled on the browser. If you haven't explicitly disabled these, then they are most likely already enabled.
3. A printed or downloaded [PDF](https://git.opengroop.org/groopi-quickstart-v0.2.6.pdf) version of this guide.  
(This is only necessary if you plan on following this guide on the same device that you plan to connect to the Groopi.)

## Step Summary

To get us up and going, these are the steps we will be taking:

1. Powering up the Groopi.
2. Connecting your browsing device to the Groopi's WIFI network.
3. Browse to the OpenGro/Op web console.
4. Logging in to the OpenGro/Op web console.
5. Changing the default password for the OpenGro/Op web console.  

That's it, so let's get going.

## Power up the Groopi

1. Make sure the SD card is solidly inserted in the Groopi.
2. Connect the sensor to any USB port on the Groopi.
3. Connect the micro USB end of the AC/DC power supply to the Groopi.
4. Plug the plug end of the AC/DC power supply into a 120v power source. Your Groopi should now power up.

The Groopi will take a few minutes to boot up. We can't move on until fully booted. I suggest waiting 5 minutes before moving on to the next steps.

## Connecting to the Groopi's WIFI network

You will be connecting to the Groopi's WIFI network the same way you would connect to any other WIFI network. Your Groopi's network name and password are labeled on the Groopi.

1. With your browsing device, search for the Groopi's WIFI network. This is usually done in your device's WIFI settings.
2. Select the Groopi's WIFI network.
3. Enter the Groopi's WIFI network password when prompted.

You should now be connected to the Groopi's WIFI network. Now you're ready to access the OpenGro/Op web console.

> ***Note:*** *While connected to the Groopi's WIFI connection, your browsing device will not have Internet access through it's WIFI connection.*

## Browse to the OpenGro/Op web console

With your browsing device connected to the Groopi's WIFI network, open up a browser and enter this IP address into the address bar:

- 10.10.10.1

This will take you to the OpenGr/Op web console login page.  

## Log in to access the OpenGro/Op web console

The login credentials are:
+ USERNAME: ***admin***
+ PASSWORD: ***opengroop***

After a successful login, you'll be directed to the *Sensors* section. This is where your sensors will be listed, showing their current readings.  
Selecting the sensor will direct you to the sensor's chart page where you can view charts based on the sensor's data, or change sensor settings.

> ***Note:*** *While current readings will be immediately stored and available for viewing, charts will be initially delayed. Hourly charts will appear after 30 minutes. Daily summary charts will appear in 2 days. This delay will occur only once, the first time a sensor is connected to the Groopi.*

## Change default password for the OpenGro/Op web console (*optional*)

Although not required, it is strongly advised that you change the default *'admin'* user password.  

1. On the main navigation, select *SETTINGS*
2. Select *USERS*
3. In the *EDIT USER* section, select the user *'admin'* (it will be the only user available)
4. Enter the new password twice, then *SUBMIT*.

#### Note on changing the *admin* password

There are currently no facilities to reset this password if forgotten. So please **do not outsmart yourself by picking a complicated password**. The objective here is to change the password from the default one provided, which is a publicly known password.

## That's it!

Now whenever you want to view your sensor data, all you have to do is join the Groopi's WIFI network, browse to the IP address above, and log into the OpenGro/Op console. Just remember that your browsing device will not have Internet access through it's WIFI while connected to the Groopi's WIFI network.  
