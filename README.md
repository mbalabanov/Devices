# Device Power Management
 
This is a system for device power management. Each powered device can be powered on and off individually. Additionally, a device manager can power multiple or all devices on and off. A type of device called BroadcastReceivers can be controlled by a remote control.

There are four classes of powered devices:
- CoffeeMaker
- TableLamp
- Radio
- Television

All devices classes are subclasses of the super-class PoweredDevices. The classes for Radio and Television inherit the class BroadcastDevices, which in turn inherits the super-class PoweredDevice. The BroadCastDevice class also implements the interface RemoteControllable and has a loose association with the RemoteControl class.

## UML Class Diagram
![Devices UML Class-Diagram](DevicesUML.png)
