#Initializing and Handling the devices

# Device Specific Functions #

  * getDeviceCount
  * getDeviceList
  * getDriverVersion
  * daqDevice


# Function Details #

_class_ **daqDevice**( deviceName )

Initializes the device with the name deviceName given from the getDeviceList() function.  deviceName is passed as a string variable and returns a device object from which additional device specific methods can be run.

### Attributes ###

> daqDevice.handle is the handle of the device given by the .dll and should never have to be used as it is an internal attribute.

> daqDevice.deviceName is the name of the device returned as a string.

> daqDevice.props is a dictionary of the device properties filled with information for    interpreting returned values and scan configurations


---


**getDeviceCount()**

Returns an integer of the number of devices currently installed on the computer

**getDeviceList()**

Returns a list of strings of names of the currently installed devices.  The names can then be used to initialize the device.

**getDriverVersion()**

Returns the current driver version of the Daq software.