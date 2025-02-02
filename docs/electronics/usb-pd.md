# An introduction to USB-PD (Power Delivery)
USB is a hellscape of different standards, capabilities and ports. From the OSSM perspective, we're concerned about the USB-PD standard which operates over the USB-C physical standard. In order to get more than 5v, both ends of the system must negotiate what voltages to use. Additionally, in order to pass more than 60w, the cable must have an e-marker defining how much wattage the cable can transmit. This can be up to 240w. The maximum capacity of any one component sets the maximum capacity for the system. In order to get these higher wattages, the USB-PD spec increases the voltage. The maximum amperage for USB-C is 5A, so in order to reach the 240w max spec, the voltage must be 48v. The highest USB-PD voltage that is still usable by the OSSM is 20v at 5a, limiting the OSSM to 100w continuous. The following are the USB-PD power options:
- 5v, 5a, 25w
- 9v, 5a, 45w
- 15v, 5a, 75w
- 20v, 5a, 100w
- 28v, 5a, 140w
- 36v, 5a, 180w
- 48v, 5a, 240w

In order for the OSSM to use USB-PD, the power supply must be capable of at least 100w, the cable must be e-marked for at least 100w and the USB-PD trigger being used must negotiate up to 20v at 5a. 