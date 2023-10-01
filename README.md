# Device Power Management
 
This is a system for the management of grid-powered devices. 

In general, any powered device can be powered on and off individually. There are two types of powered devices:
- GridPoweredDevices
- BatteryPoweredDevices

There are four types of grid-powered devices:
- CoffeeMaker
- TableLamp
- Radio (BroadCastReceiver)
- Television (BroadCastReceiver)

There is one type of BatteryPoweredDevice:
- RemoteControl

The GridPoweredDeviceManager can power multiple or all grid-powered devices on and off. Radio and Television are a type of device called BroadcastReceivers can be controlled by a RemoteControl. The RemoteControl is a battery-powered device, it cannot be controlled by the GridPoweredDeviceManager but it can be used to control the Radio and the Television.

All device-classes are subclasses of the super-class PoweredDevices. The classes BatteryPoweredDevice and GridPoweredDevice are subclasses of PoweredDevice. The classes CoffeeMaker, TableLamp are direct decendants of GridPoweredDevice, while the classes for Radio and Television decend from the class BroadcastDevices, which in turn decends from the super-class GridPoweredDevice. The BroadCastDevice class also implements the interface RemoteControllable and has a loose association with the RemoteControl class.

## UML Class Diagram
![Devices UML Class-Diagram](DevicesUML.png)
