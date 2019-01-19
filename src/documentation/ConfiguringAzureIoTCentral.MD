#Configuring Azure IoT Central

Assuming you've followed the instructions up to this point and have connected your MXChip device, you now having a working device set-up in Azure IoT Central which is sending you data.  If you want - you're done!  But of course, where's the fun in that?

## Choosing What's Next

Deciding how to configure your IoT Central App next is completely up to you, but here's the big areas you'll want to consider:

### Dashboard

Your IoT Central's Dashboard is the first page that will open up when you open your App and ideally it should serve as a "Single Pane of Glass" for your project.  Think of it as they main place you'll spend your time (especially when you demonstrate your app to friends and colleagues) and you want it configured so you simply "drill in" into your device(s) from it.

#### What can you do here?

A few ideas:

+ **Images**
  + Nothing personalizes a dashboard and shows "you mean business", by adding a few custom images.  The image control is simple and easy to use, to upload one of your own images into the dashboard.
+ **Show your Device's Location on a Map**
  + You can show your device's location on a map on your dashboard.  The MXChip IoT Devkit template comes with a location property, but it's typically not updated by the device.  The easiest step is to create your own Location property on the device template and update it manually by entering an address or Lat/Long into it.
+ **KPI**
  + The first role of any operational IoT dashboard is typically "show me what's on fire"; ie, show me what I MOST need to know.  KPI's do this best.  Experiment with what telemetry you can show and especially look at which Aggregate function to use (via the Gear icon next to each Measurement in the Configure KPI slider).
+ **Last Known Value**
  + While the KPI control shows the output of an aggregate, the Last Known Value control shows ... [wait for it] ... a Measurement's Last Known Value.  This can be helpful for something like Temperature when what you're interested in is the raw, last value that the MXChip device recorded.

Of course - there's many other options here.  Review the [on-line documentation](https://docs.microsoft.com/en-us/azure/iot-central/howto-configure-homepage) for further instructions and assistance.


### Device Rules and Actions

Taking action on the information your MXChip is providing you about the world can often be the most compelling part of an IoT project.  Azure IoT Central's rules and actions are easy to use and well documented [here](https://docs.microsoft.com/en-us/azure/iot-central/tutorial-configure-rules).

The simplest action is sending an e-Mail, which IoT Central can do for you out-out-box.  I'm a big fan of using the Microsoft Flow integration.  If you're not familiar with Microsoft Flow, it's a consumer-based workflow integration which enables simple to complex handling of all types of workflows, and for most scenerios requires NO CODING.  For example, if you wanted to send yourself a text message, you could use Microsoft Flow and one of its SMS Provider Connectors (Twilio is my favorite, though it does require you to set-up a Twilio account) to do so.

Click [here](https://docs.microsoft.com/en-us/azure/iot-central/howto-add-microsoft-flow) for further documentation on how to integrate an IoT Central rule/action with Microsoft Flow.

