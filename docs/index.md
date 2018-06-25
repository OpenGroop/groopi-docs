OpenGro/Op User Manual
==================

## Table of contents

1. [Login / Logout](#login_off)
2. [Sensors](#sensors)
	1. [Sensor Charts](#sensor_charts)
		1. [Hourly Charts](#hourly_charts)
		2. [Daily Charts](#daily_charts)
	2. [Sensor Settings](#sensor_settings)
		1. [Sensor ID](#sensor_id)
		2. [Sensor Alias](#sensor_alias)
		2. [Unit of Measure](#uom)
3. [Settings](#settings)
	1. [Network Settings](#network_settings)
		1. [Wireless Acces Point](#network_ap)
		2. [Local Network](#network_local)
		3. [Remote Network](#network_remote)
	2. [User Settings](#user_settings)
		1. [Add User](#user_add)
		2. [Edit User](#user_edit)
	3. [Cloud Account Settings](#cloud_account_settings)
	4. [Backup / Restore Data](#backup_restore)
4. [Support](#support)

<a name="login_off"></a>
## Login / Logoff
Logging in is a straightforward process. Type in your username and password.  
OpenGro/Op currently implements a two second pause between login attempt and logging in. After succesfull login, you'll be directed to your [Sensors](#sensors).  
OpenGro/Op requires you to have cookies enabled in your browser. This is to facilitate user login session information and clears itself after thirty minutes of inactivity or logging out.  
As well, OpenGro/Op requires javascript to be enabled on your browser.
<a name="sensors"></a>
## Sensors
All connected sensors will be listed here with their latest reading. This reading will be no more than a minute old and can be considered a "real time" reading. This page does not refresh automatically, so if you want the most current reading, this page must be refreshed.  
Sensors are listed alphabetically by their [sensor alias](#sensor_alias). Clicking the sensor alias will take you to the sensor's chart section where the sensor's historical readings and settings are accessed.

<a name="sensor_charts"></a>
### Sensors: Charts
Sensor charts are reached by clicking their respective alias links on the Sensor section.  
There are two types of charts available. Hourly charts and daily charts. Hourly charts offer up granular readings while daily charts offer daily summaries.
Both types of charts require at least two points of data to te rendered. This means hourly charts will not render until 30 
minutes of data has been recorded. Daily charts, unfortunately, two days.
<a name="hourly_charts"></a>
#### Hourly Charts
Hourly charts will chart temperature, humidity, and light levels hourly for 1, 2, 3, and 7 days.  
Each chart has a different resolution:

| Hours | Days | Resolution |
|:------|:-----|:-----------|
| 24    | 1    | 15 minutes |
| 48    | 2    | 30 minutes |
| 72    | 3    | 45 minutes |
| 144   | 7    | 90 minutes |


<a name="daily_charts"></a>
#### Daily Charts
Daily charts serve up summaries of daily averages. There are 5 charts available. 7, 14, 30, 60, and 90 days. The first chart displays temperature day/night averages, while the second chart displays humidity day/night averages.

<a name="sensor_settings"></a>
### Sensor Settings
The follwing are settings which are used to define sensors.

<a name="sensor_id"></a>
#### Sensor ID
The sensor ID is the sensor's serial number. Every sensor built will hava a unique ID. This ID is used to identify the sensor for both the RPi installations as well as cloud accounts. Therefore this ID is static and cannot be changed. 

<a name="sensor_alias"></a>
#### Sensor Alias
The sensor alias is a configurable name that you can give your sensor to easily identify it. By default, OpenGro/Op will assign the sensor's ID as it's alias. You are encouraged to change it to a more suitable and identifiable name, such as 'transplanting tent' or 'flowering room'.  
Changing the alias will not alter the data associated with the sensor. Only [deleting](#sensor_delete) can alter the data.
<a name="uom"></a>
#### Tempurature Unit of Measure
This sets the sensor's temperature unit of measure between Celsius and Fahrenheit. This does not affect how the sensor's tempurature data is stored. It only affects how tempurature is displayed.

<a name="sensor_delete"></a>
#### Sensor Delete
This deletes all the data associated with the sensor. You must enter the sensor ID or alias (cap-sensitive) to confirm data deletion. This process is irreversable and should be treated with caution.  
One use case for this might be that the sensor is being moved to another area or room and you would like to start tracking it's data fresh. This allows you to remove all previous data associated with the sensor to allow a clean start.

<a name="settings"></a>
## Settings

<a name="network_settings"></a>
### Network Settings

<a name="network_ap"></a>
#### Wireless Access Point
Displays credentials used to connect the Groopi's WIFI access point.

<a name="network_local"></a>
#### Local Network
Displays local network connections information for Ethernet and WIFI interfaces.

<a name="wifi_config"></a>
##### Configure WIFI Client
Choose a WIFI network to connect to. You will be prompted to enter it's password.

<a name="network_remote"></a>
#### Remote Network
Displays information needed to access OpenGro/Op remotely. 

<a name="user_settings"></a>
### Users
Multiple users can be assigned access to the OpenGro/Op console.  
By default, only the _admin_ user has access to the Settings section. This goes for [sensor settings](#sensor_settings) as well.  All new users created will only have read access to OpenGro/Op. They will only be able to read sensor charts.

<a name="user_add"></a>
#### Add User
Adds new users to OpenGro/Op.

<a name="Edit User"></a>
#### Edit User
Edits user's password, or deletes user from the system. If looking to change the user's name, delete the user, then create a new user with the new name.

<a name="cloud_account_settings"></a>
### Cloud Account Settings
Server credentials to access a cloud account.

<a name="backup_restore"></a>
### Backup / Restore Data
Backup and/or restore all database data to usb drive. Drive must be formatted as FAT32 drive. Insert the drive into one the RPi's usb port and refresh the page. OpenGro/Op will automatically detect the drive and present the option to backup the database.  
If a drive contains a valid OpenGro/Op backup, that backup can also be restored. If a drive contain multiple backups, OpenGro/Op will restore the most current backup.

<a name="support"></a>
## Support
Contains contact and support information.

