# Device Power Management
 
This is a system for the management of grid-powered devices. 

In general, any powered device can be powered on and off individually. There are two types of powered devices:
- Grid-powered devices
- Battery-powered devices

There are four types of grid-powered devices:
- CoffeeMaker
- TableLamp
- Radio
- Television

There is one type of battery-powered device:
- RemoteControl

A device manager can power multiple or all grid-powered devices on and off. A type of device called BroadcastReceivers can be controlled by a RemoteControl. The RemoteControl is a battery-powered device, it cannot be controlled by the device manager but it can be used to control the Radio and the Television.

All devices classes are subclasses of the super-class PoweredDevices. The classes for Radio and Television inherit the class BroadcastDevices, which in turn inherits the super-class PoweredDevice. The BroadCastDevice class also implements the interface RemoteControllable and has a loose association with the RemoteControl class.

## UML Class Diagram
![Devices UML Class-Diagram](DevicesUML.png)
