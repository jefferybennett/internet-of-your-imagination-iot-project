# Creating Your First IoT Central App

- [Creating Your First IoT Central App](#creating-your-first-iot-central-app)
    - [What's an IoT Central App?](#whats-an-iot-central-app)
    - [Create the App](#create-the-app)
        - [Navigate to the IoT Central Application Manager](#navigate-to-the-iot-central-application-manager)
        - [Complete the New Application form.](#complete-the-new-application-form)
    - [Next steps](#next-steps)

## What's an IoT Central App?

Azure IoT Central enables a single organization to create multiple "Apps" such that, for example, multiple departments could create completely seperate IoT Central App instances in the same Azure tenant.

Each App has its own separate device templates, devices and settings, as well as an unique URL for users to access.

## Create the App

### Navigate to the IoT Central Application Manager

The Application Manager enables you to both create new IoT Central Apps and to access existing ones.

- [ ] Navigate to the [Azure IoT Central Application Manager](https://apps.azureiotcentral.com/).
- [ ] If you're not already, logon to the Application Manager using the correct credentials associated to your Microsoft Azure environment.
- [ ] To start creating a new Azure IoT Central application, choose New Application:

![alt-text](src/images/IC-ApplicationManager.png)

### Complete the New Application form.

- [ ] Choose the Paid payment plan.
    > Note:
    >
    > Currently you can use up to 5 devices in IoT Central for free.  If you select the Free payment plan, your trial will only last 7 days.
- [ ] Choose the Sample Devkits template.
    > Note:
    >
    > The Sample Devkits template provides a completed device template for the MXChip board.
- [ ] Choose a friendly application name.
    -  Azure IoT Central generates a unique URL prefix for you. You can change this URL prefix to something more memorable.
- [ ] Keep the default directory.
    -   For Microsoft Employees, this should be "Microsoft (microsoft.onmicrosoft.com)".
- [ ] Select the correct Azure Subscription.
    -   For Microsoft Employees, this should be "Microsoft Azure Internal Consumption".
- [ ] Select the closest Azure region to you.
- [ ] When you're finished and believe your entries are correct, click the Create button to finalize the app creation.

![alt-text](src/images/IC-NewApplication.png)

After your App is created, you'll be immediately logged into it.

CONGRATULATIONS!!!  Your Azure IoT Central is now CREATED!

## Next steps

Now that we've created our IoT Central app, we can focus on connecting our MXChip board to IoT Central.  Click [here](ConnectingTheMXChip.MD) to begin!