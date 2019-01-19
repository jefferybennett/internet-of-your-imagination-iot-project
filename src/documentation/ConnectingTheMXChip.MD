# Connecting the MXChip Board

- [Connecting the MXChip Board](#connecting-the-mxchip-board)
    - [Before you Begin](#before-you-begin)
    - [Add a real device to your App](#add-a-real-device-to-your-app)
    - [Prepare the MXChip device](#prepare-the-mxchip-device)
    - [View the telemetry](#view-the-telemetry)

## Before you Begin

To complete the steps in this article, you need the following:

- An Azure IoT Central application created from the Sample Devkits application template. Click [here](CreateYourFirstIoTCentralApp.MD) if you haven't already created your App.
- A MXChip device.

> Note:
> 
> While your IoT Central App is immediately available after you create it, it takes a few minutes to completely provision completely.  It's possible you'll run into an "Application Still Provisioning" message on certain pages until it's complete.

## Add a real device to your App

In your Azure IoT Central App, add a "real" device from the **MXChip** device template and make a note of the device connection details (Scope ID, Device ID, and Primary key).  You'll want to save these details temporarily in an application like Notepad for easy access as you go through this process.

> Note:
> 
> A simulated device is automatically created for each IoT Central device template.  IoT Central automatically simulates its data based upon the Measurements configured for it in its device template.
> 
> A real device is a physical device which will be connected to IoT Central.

![alt-text](src/images/IC-CreateRealDevice.png)

- [ ] Add a **real device** in Azure IoT Central.
    - [ ] If you're at your IoT Central Home Page, click "View All Devices".
    - [ ] If you're on the Device Explorer, click on **+New > Real** to add a real device.
    - [ ] Enter the Device Id (should be lower case) or use the suggested Device Id.
    - [ ] Enter the Device Name or use the suggested name.
    ![alt-text](src/images/add-device.png)
    - [ ] Get connection details such as Scope ID, Device ID, and Primary key for the added device by clicking **Connect** on the device page.
    - [ ] Make sure to save these details, as you will temporarily get disconnected from the internet as you prepare the DevKit device.

## Prepare the MXChip device

> Note:
> 
>  If you have previously used the device and have wifi credentials stored and would like to reconfigure the device to use a different WiFi network, connection string, or telemetry measurement, press both the A and B buttons on the board simultaneously. If it doesn't work, press reset button and try again.

- [ ] Download the firmware titled 'Azure IoT Central - Sample firmware v.2.0.0' for the MXChip from the [releases](https://github.com/Azure/iot-central-firmware/releases) page on GitHub.
- [ ] Connect the DevKit device to your development machine using a USB cable. In Windows, a file explorer window opens on a drive mapped to the storage on the DevKit device. For example, the drive might be called AZ3166 (D:).
- [ ] Drag the iotCentral.bin file onto the drive window. When the copying is complete, the device reboots with the new firmware.

When the DevKit device restarts, the following screen displays:

```text
Connect HotSpot:
AZ3166_??????
go-> 192.168.0.1 
PIN CODE xxxxx
```
> Note:
> 
> If the screen displays anything else, reset the device and press the A and B buttons on the device at the same time to reboot the device.

- [ ] The device is now in access point (AP) mode. You can connect to this WiFi access point from your computer or mobile device.

- [ ] On your computer, phone, or tablet connect to the WiFi network name shown on the screen of the device. When you connect to this network, you do not have internet access. This state is expected, and you are only connected to this network for a short time while you configure the device.

- [ ] Open your web browser and navigate to [http://192.168.0.1/start](http://192.168.0.1/start). The following web page displays:
    ![alt-text](src/images/mxchip-configpage.png)

- [ ] In the web page:
    - [ ] Add the name of your WiFi network
    - [ ] Your WiFi network password
    - [ ] PIN CODE shown on the device LCD
    - [ ] The connection details Scope Id, Device Id, and Primary key of your device (you should have already saved this following the steps)
    - [ ] Select all the available telemetry measurements.

- [ ] After you choose **Configure Device**, you'll see this page:
    ![alt-text](src/images/mxchip-deviceconfigured.png)

- [ ] Press the **Reset** button on your device.

## View the telemetry

When the DevKit device restarts, the screen on the device shows:

- The number of telemetry messages sent.
- The number of failures.
- The number of desired properties received and the number of reported properties sent.
> Note:
> 
> If the device appears to be looping during connect check if the device is Blocked in IoT Central, and Unblock the device so it can connect to the app.

Shake the device increment the number of reported properties sent. The device sends a random number as the Die number device property.

You can view the telemetry measurements and reported property values, and configure settings in Azure IoT Central:

- [ ] Use Device Explorer to navigate to the Measurements page for the real MXChip device you added:
    ![alt-text](src/images/mxchip-realdevicenew.png)

- [ ] On the **Measurements** page, you can see the telemetry coming from the MXChip device:
    ![alt-text](src/images/ic-devicetelemetrynew.png)

- [ ] On the **Properties** page, you can view the last die number and the device location reported by the device:
    ![alt-text](src/images/ic-devicepropertynew.png)

- [ ] On the **Settings** page, you can update the settings on the MXChip device:
    ![alt-text](src/images/ic-devicesettingsnew.png)

- [ ] On the **Dashboard** page, you can see the location map:
    ![alt-text](src/images/ic-devicedashboardnew.png)