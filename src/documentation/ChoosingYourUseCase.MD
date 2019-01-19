# Choosing Your Use Case

- [Choosing Your Use Case](#choosing-your-use-case)
  - [Thinking Deeply about IoT](#thinking-deeply-about-iot)
    - [Understanding and Interacting](#understanding-and-interacting)
  - [Use Case Examples](#use-case-examples)
  - [Selecting Your Use Case](#selecting-your-use-case)
  - [MXChip Board Capabilities](#mxchip-board-capabilities)
    - [Measurements](#measurements)
      - [Telemetry](#telemetry)
      - [States](#states)
      - [Events](#events)
    - [Settings](#settings)
      - [Numeric settings](#numeric-settings)
      - [Toggle settings](#toggle-settings)
      - [Properties](#properties)

## Thinking Deeply about IoT

While there's a million definitions for the term "IoT", consider this one as we begin thinking about your project use case:

- **IoT**: The "Internet of Things" refers to various types of non-traditional compute devices which enable people and organizations to both understand and interact with the new world in new ways.

### Understanding and Interacting
As you begin to think about your project's use case, think about ways that would be personally compelling for you to either understand or interact with the world in a way you haven't before.

Next, take these ideas and compare them with the [capabilities](#mxchip-board-capabilities) of the MXChip board.  You'll see that what the MXChip board is best at is **understanding** the world through various sensors.

The MXChip board has a whole host of sensors with which we can use to "understand" the world better.  For example, it has temperature, humidity and barometric sensors, which could enable you to monitor a space whose climate must be closely maintained.

## Use Case Examples

Here are some examples of use cases which people have used in their Internet of Your Imagination IoT project:

- **Internet of Your Cigars - Humidor Monitoring**
  - If you're someone who enjoys cigars, you know that keeping them at the right temperature and humidity is critical.  In this project, the creator took two MXChip devices, placed one inside their humidor and the other immediately outside of it, to monitor the temperature and humidity inside and outside of their humidor.  They then set-up a simple alert inside IoT Central to notify them when the environmental levels were outside the preferred zone.  Pretty cool!
- **No More Frozen Pipes - Garage Monitoring**
  - If you live in a colder climate, you're probably familiar with the risk and consequences of frozen pipes.  For this project's creator, pipes typically will freeze in winter if their garage door is left open (teenagers may or may not be involved).  By monitoring the temperature of their garage and having IoT Central send an alert if the temperature falls below a key threshold, the project's creator was able to take quick action to stay off an expensive visit from the plumber.
- **Turn off the heat! - Yoga Studio Monitoring**
  - This project's creator owns a Yoga Studio and has instructors that at the end of day, quite understandbly, are are 'blissed out' and forget to turn the heat down.  Keeping a yoga studio is important, but it tends to get expensive and a bit needless when there's no one there.  By setting up a MXChip in the studio, the project's creator was able to keep an eye on the temperature and know when someone had forgotten to turn off the heat at the end of the day.

## Selecting Your Use Case

There's many factors involved with selecting your project's use case, but here's the key ones:

+ **Wifi Access**
  + The MXChip device relies upon Wifi to communicate through the internet to IoT Central.
+ **Power**
  + To keep things simple, the MXChip relies upon a steady power source provided by a USB 2.0 to Micro B Male cable, which is plugged into a wall socket.  Luckily, such cables are incredible common and even longer cables are typically pretty cheap.
+ **MXChip Sensors**
  + The MXChip IoT devkit board comes with a number of on-board sensors (outlined below).  What are some ideas of what you can do with them?
    + **Humidity** - Tracking humidity can be incredibly useful for any number of scenarios: monitoring a greenhouse, the humidity in your house or a paricular room with things that are sensitive to it.
    + **Temperature** - Clearly a fan favorite, there's a million good reasons to measure temperature.
    + **Barometric Pressure** - Before the days of weather satelites, barometric pressure was one of the key predictors of a storm coming.  With the ability to measure barometric pressure, temperature and humidity, your MXChip isn't a bad tiny little weather station.
    + **Magnetometer** - Not a sensor I've personally played with, the MXChip's magnotemeter sensor measures the strength and direction of magnetic fields.  One imagines it might potentially spike for someone with an especially *electric* personality.
    + **Accelerometer** - The MXChip's accelerometer sensor can measure the speed and direction of the device's acceleration.  So for example, you couldn't use this to measure the speed of a car, but you could measure a "quick stop" (assuming of course you had a Wifi source and power adapter for the MXChip in your car).  This is a great sensor to detect something being moved.
    + **Gyroscope** - The MXChip's gyroscope measures the MXChip's attitude - its orientation to the world, in the X / Y / Z axis.  Plenty of things are sensitive to not being tipped over, for example.

## MXChip Board Capabilities

### Measurements

#### Telemetry
| Field name	| Units	 | Minimum | Maximum	| Decimal places |
| ------------- | :----- | :------ | :------ | :------------- |
| humidity	    | %      | 0	   | 100	 | 0              |
| temp	        | °C     | -40	   | 120	 | 0              |
| pressure	    | hPa	 | 260     | 1260    | 0              |
| magnetometerX	| mgauss | -1000   | 1000	 | 0              |
| magnetometerY	| mgauss | -1000   | 1000    | 0              |
| magnetometerZ	| mgauss|	-1000|	1000|	0|
| accelerometerX |	mg|	-2000|	2000|	0|
| accelerometerY |	mg|	-2000|	2000|	0|
| accelerometerZ |	mg|	-2000|	2000|	0|
| gyroscopeX|	mdps|	-2000|	2000|	0|
| gyroscopeY|	mdps|	-2000|	2000|	0|
| gyroscopeZ|	mdps|	-2000|	2000|	0|

#### States

Name	Display name	NORMAL	CAUTION	DANGER
DeviceState	Device State	Green	Orange	Red

| Name	| Display Name	 | NORMAL| CAUTION	| DANGER |
| ------------- | :----- | :------ | :------ | :------------- |
| DeviceState	    | Device State     | Green	   | Orange	 | Red             |

#### Events

| Name	| Display name	 | 
| ------------- | :----- |
| ButtonBPressed	    | Button B Pressed      | 

### Settings

#### Numeric settings
| Display name	| Field name	 | Units| Decimal Places	| Minimum | Maximum | Initial |
| ------------- | :----- | :------ | :------ | :---- | :---- | :---- |
| Voltage	    | setVoltage     | Volts	   | 0	 | 0  | 240             | 0 |
| Current	    | setCurrent     | Amps	   | 0	 | 0  | 100             | 0 |
| Fan Speed	    | fanSpeed     | RPM	   | 0	 | 0  | 1000             | 0 |

#### Toggle settings
| Display name	| Field name	 | On text| Off text	| Initial | 
| ------------- | :----- | :------ | :------ | :---- |
| IR	    | activateIR    | ON	   | OFF	 | Off |

#### Properties
| Type	| Display name	 | Field name| Data type | 
| ------------- | :----- | :------ | :------ |
| Device property	    | Die number    | dieNumber	   | number	 |
| Device property	    | Device Location    | location	   | location	 |
| Text	    | Manufactured In   | manufacturedIn   | N/A	 |


