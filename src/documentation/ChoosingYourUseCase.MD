# Choosing Your Use Case

- [Choosing Your Use Case](#choosing-your-use-case)
    - [Thinking Deeply about IoT](#thinking-deeply-about-iot)
        - [Understanding and Interacting](#understanding-and-interacting)
        - [Some New, Important Terms for You to Know](#some-new-important-terms-for-you-to-know)
    - [Use Case Ideas](#use-case-ideas)
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

### Some New, Important Terms for You to Know



## Use Case Ideas

## Selecting Your Use Case




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


