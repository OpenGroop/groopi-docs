# Groopi Quickstart Guide

This quickstart guide will guide you through the process of getting your Groopi up and running quickly. But before we start, there are few requirements.


## Requirements

1. A WIFI cabable device with a web browser. This can be on a phone, tablet, laptop, etc.., anything with a web browser.
2. Javascript and cookies must be enabled on the browser. If you haven't explicitly disabled these, then they are most likely already enabled.
3. Downloaded PDF version of this guide.  
(This is only necessary if you plan on follwing this guide on the same device that you plan to connect to the Groopi.)

## Step Summary

To get us up and going, these are the steps we will be taking:

1. Powering up the Groopi.
2. Connecting your browsing device to the Groopi's WIFI network.
3. Browse to the OpenGro/Op web console.
3. Configuring your browser to accept security warning.
4. Logging in to the OpenGro/Op web console.
5. Changing the default password for the OpenGro/Op web console. (*optional*)

That's it, so let's get going.

## Power up the Groopi

1. Make sure the SD card is inserted correctly. It should be inserted with the pins facing in and towards the RPI.
2. Connect the sensor to any USB port on the Groopi.
3. Connect the micro USB end of the AC/DC power supply to the Groopi.
4. Plug the plug end of the AC/DC power supply into a 120v power source. Your Groopi should now power up.

The Groopi will take a few minutes to boot up. We can't move on until fully booted. I suggest waiting 5 minutes before moving on to the next steps.

##Connecting to the Groopi's WIFI network

You will be connecting to the Groopi's WIFI network the same way you would connect to any other WIFI network. Your Groopi's network name and password are labeled on the Groopi.

1. With your browsing device, search for the Groopi's WIFI network. This is usually done in your device's WIFI settings.
2. Select the Groopi's WIFI network.
3. Enter the Groopi's WIFI network password when prompted.

You should now be connected to the Groopi's WIFI network. Now you're ready to access the OpenGro/Op web console.

## Browse to the OpenGro/Op web console

With your browsing device connected to the Groopi's WIFI network, open up a browser and enter into it's address bar:

- https://10.10.10.1

You will receive an ominous warning from your browser claiming that the connection is *'untrusted'* or *'not private'*. **This warning can be ignored and bypassed.** The next section covers dealing with this warning.

## Configure browsers to accept security warning

When accessing the OpenGro/Op console for the first time, you will receive a warning claiming that the site is *'untrusted'* or *'not private'*. As ominous as this may sound, we can ignore this warning and move on. But to do that, we must let the browser know that we trust the connection. Different browsers have different ways to do this.

### Chrome

On the warning page:

1. select *'ADVANCED'*
2. then, select *'Proceed to 10.10.10.1 (unsafe)'*

### Firefox

On the warning page,

1. select *'Advanced'*
2. then, select *'Visit site anayway'*

### Safari

On the warning page,

1. select *'Show Details'*
2. then, select *'visit this website'*

#### Note on browser warnings
This warning will appear the first time we access OpenGro/Op for each browser. Bypassing this warning on Chrome will not automatically bypass it on Firefox or Safari. Each browser type must remember it's own bypass setting. This also applies across browsing devices.   

After bypassing the warning, we will be presented with the *Login* page.

## Log in to access the OpenGro/Op web console

With WIFI connections made and browser warnings bypassed, we are now ready to log in.

+ USERNAME: ***admin***
+ PASSWORD: ***opengroop***

After a successfull login, you'll be directed to the *Sensors* section. This is where your sensors will be listed, showing their current readings.  
Selecting the sensor will direct you to the sensor's chart page where you can view charts based on the sensor's data, or change sensor settings. 

#### Notes on readings and viewing charts

While current readings will be immediately stored and available for viewing, hourly charts will not be available for the first 30 minutes. Daily charts will not be available for 2 days:(.

## Change default password for the OpenGro/Op web console (*optional*)

Although not required, it is suggested that you change the default *'admin'* user password.  

1. On the main navigation, select *SETTINGS*
2. Select *USERS*
3. In the *EDIT USER* section, select the user *'admin'* (it will be the only user available)
4. Enter the new password twice, then *SUBMIT*.

#### Note on changing the *admin* password

There are currently no facilities to reset this password if forgotten. So please **do not outsmart yourself by picking a complicated password**. The objective here is to change the password from the default one provided, which is a publicly known password.

## That's it!

Now whenever you want to view your sensor data, all you have to do is join the Groopi's WIFI network, browse to the IP address above, and log into the OpenGro/Op console. Just remember that your browsing device will not have internet access while connected to the Groopi's WIFI network.  

## What's next?

The Groopi has a few more features that are worth exploring. All of which are covered in the [Opengro/Op User Manual](/opengroop_user_manual/).

#### Local network connections

The Groopi can connect to existing local networks by either WIFI, ethernet, or both. By connecting the Groopi to an existing network, you do not have to switch networks to access the OpenGro/Op web console. It will hava an address on that network.

#### Remote network connection

If you have the Groopi connected to a local network that has internet access, then the Groopi can also be accessed remotely, off-site.

#### Cloud data storage
  
Sensor data can be pushed to the cloud for storing and viewing.

#### User magament

Users can be added to the system to access sensor data.


For a detailed a reference on the OpenGro/Op web console, visit the  [Opengro/Op Reference Manual](/opengroop_reference_manual/).


