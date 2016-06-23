# Features

## Dashboard
The Cayenne dashboard (online and mobile) is the main screen where you can setup, customize, monitor, manage and control your connected devices.

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160601123646/LightSwitch-RPI-todashboard.jpg" width="600" height="383" alt="Light Switch Dashboard"></p>

From the Cayenne dashboard you can:

+ Add [Raspberry Pis](http://www.cayenne-mydevices.com/CayenneStaging/docs#raspberry-pi-single-board-computers), [Arduino boards](http://www.cayenne-mydevices.com/CayenneStaging/docs#arduino-microcontrollers), [sensors](http://www.cayenne-mydevices.com/CayenneStaging/docs#sensors-supported-hardware), [actuators](http://www.cayenne-mydevices.com/CayenneStaging/docs#actuators-supported-hardware) and [extensions](http://www.cayenne-mydevices.com/CayenneStaging/docs#extensions-supported-hardware).
+ Fully customize your dashboard with [drag-and-drop widgets](http://www.cayenne-mydevices.com/CayenneStaging/docs#drag-and-drop-widgets-dashboard).
+ View [device and sensor data history](http://www.cayenne-mydevices.com/CayenneStaging/docs#device-and-sensor-history-dashboard).
+ Setup [automatic triggers](http://www.cayenne-mydevices.com/CayenneStaging/docs#rules-engine) and receive [notification alerts](http://www.cayenne-mydevices.com/CayenneStaging/docs#notifications).
+ [Schedule actions](http://www.cayenne-mydevices.com/CayenneStaging/docs#scheduling) and commands.
+ [Create IoT projects](http://www.cayenne-mydevices.com/CayenneStaging/docs#projects).
+ Remotely manage devices and sensors.


### Drag-and-drop widgets
Cayenne uses widgets to visualize devices, their data, status and actions. Every device, sensor and actuator that gets added in Cayenne has one or more widgets associated depending on the hardware capabilities. Widgets are added to the Device list on the left hand side and to each device’s Dashboard.

Widgets can be be re-arranged on your dashboard by drag and dropping them anywhere. To move a widget, place your mouse or finger at top middle area of widget. Then tap and move the widget where you want it on your dashboard.

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160602132429/Widget-Move.jpg" width="600" height="319" alt="Arduino IDE Port Selection"></p>


### Widget settings

A variety of widget parameters can be customized by the user. Access the widget settings by selecting the wheel in the upper right of the widget. In here you can change the widget type, change the min/max values and more.

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160602132209/Project-WidgetSettings.jpg" width="300" height="330" alt="Project Widget Settings"></p>


## Visualization

Cayenne stores historical data that enables you to see meaningful patterns of behavior to help understand and guide improvements on your IoT projects and the devices and sensors connected.


### Live Data

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160602132957/Sensor-Live.jpg" width="600" height="244" alt="Sensor Live"></p>


### Data History

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160602133036/Sensor-History.jpg" width="600" height="244" alt="Sensor History"></p>


### Filtering visualization

From the data history graph, you have the ability to filter by different timeframes. Depending upon the timeframe you have selected, the data display will update to show you more or less detail.

You can select from any of the preset ranges available. The ranges shown to you here may depend upon the data currently available for the device. For example, if the device was recently added you may not see the option to select the yearly options. Some options such as **minutes** and **year to date** will always be present. Custom filtering options will added soon.

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160602134448/Line-Chart-filtering.png" width="600" height="220" alt="Line Chart Filtering"></p>


### Downloading data history

Coming soon you will be able download data history.


## Projects

The Projects feature allows you to combine widgets from any combination of devices into one custom dashboard called a Project. Each project has its own set of triggers and scheduled events that you can be setup.


### Creating a Project

To begin creating a new project click the **+ Create New Project** entry in the navigation menu or expand the **Add** menu and select the **Project** option.

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160601122359/AddNew.jpg" width="260" height="252" alt="Add New Device"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160602135511/CreateNewProject.jpg" width="155" height="42" alt="Create New Project"></p>


#### Naming the project

In order to create your new project, you must give the dashboard a unique name. Giving your project a name is the only required step for project creation.

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160602135634/Projects-Name.jpg" width="260" height="43" alt="Projects Name"></p>

After creating your new project, you will see a blank canvas. From here, you can start populating your new project dashboard with widgets from any of your devices.

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160602135744/Projects-Default.jpg" width="600" height="358" alt="Projects Default"></p>


#### Adding widgets

You can customize your project by adding widgets at any time. When adding widgets, you can add widgets associated with any existing device in your device list or you can add new devices that will then be added to your project as well as listed in the device list.


#### Add single widget

You can click and drag a single widget from a device into the device list area. The added widget appears in the project and the widget container clearly indicates which device this widget is associated with.

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160601131032/Arduino-TMP36.jpg" width="600" height="336" alt="Arduino TMP36"></p>


#### Adding multiple widgets

To add more than one widget at a time, you can drag the device from the device list into the dashboard area. This will allow the user to add multiple widgets associated with that device at one time.

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160602140608/Projects-MultipleWidget.jpg" width="600" height="412" alt="Multiple Widgets"></p>

After selecting some or all the widgets you would like to add from a device, they appear on the Project dashboard.

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160602140649/Projects-MultipleWidget-Dashbioard.jpg" width="600" height="358" alt="Multiple Widgets on Dashboard"></p>


#### Deleting widgets

To remove a widget from a project, click on the **cogwheel** icon in the top right corner of the widget, then click **Remove from project**.

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160602141024/Project-RemoveWidget.jpg" width="300" height="330" alt="Remove Widget"></p>

**Note:** This only removes the widget from this project. It doesn’t remove the widget from other projects or from Cayenne.


### Editing and deleting projects

To edit a project name or delete a project click on the cogwheel icon next to your Project Name.

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160601130027/Configure.jpg" width="230" height="183" alt="Configure"></p>


## Scheduling

Cayenne allows you to create scheduled events for Raspberry Pis, Arduinos, sensors and actuators connected. A scheduled event can have one or more actions added to it.

### Setting up scheduled events

Let’s create our first scheduled event. We’ll turn off the light at 10 pm every night.

1. To begin creating an Event, open the feature by selecting **Add New** and then **Event**.<br/>
   <p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160601122359/AddNew.jpg" width="260" height="252" alt="Add New Device"></p>
2. The Create New Event screen appears.
   <p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160602144155/ScheduleEvent-00.jpg" width="345" height="365" alt="Schedule Event"></p>

From here, you can fill in all the details required for creation of your scheduled event. When creating a new scheduled event, the empty screen serves as an overview of the creation process.

**Example event**
Let’s create an example event to show you how easy it is. We’ll create the following event: At 10 pm turn off the lights and turn off the fan.

1. Let’s begin by giving our scheduled event a name. Enter **“At 10 pm, Turn off Light and Fan”** into the **Event title** field.
   <p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160602144407/ScheduleEvent-01.jpg" width="345" height="365" alt="Schedule Event"><br/><br/></p>
   
2. In the Date and Time fields, enter the date you want to start the scheduled event and the time.
   <p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160602144430/ScheduleEvent-02.jpg" width="345" height="365" alt="Schedule Event"><br/><br/></p>
   
3. Select the Timezone of when you want the scheduled event to run. By Default, the scheduled event runs in the **default browser timezone** of the computer or phone you are on.
   <p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160602144501/ScheduleEvent-03.jpg" width="346" height="400" alt="Schedule Event"><br/><br/></p>
   
4. Select how often you want the scheduled event to occur. By default, the scheduled event only occurs one time. For this example we will have the scheduled event happen Every Day. Select the **Repeat** frequency and choose the **Every Day** option.
   <p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160602144544/ScheduleEvent-04.jpg" width="346" height="400" alt="Schedule Event"><br/><br/></p>
   
5. You can optionally choose to receive notifications whenever this event runs. Events can be delivered by email and/or text message. For this example, we will choose to receive notification by email and text message. Select the checkbox next to each option and enter the phone number and email address you would like to receive the notification into the appropriate fields.
   <p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160602144636/ScheduleEvent-05.jpg" width="346" height="410" alt="Schedule Event"><br/><br/></p>
   
6. To complete your scheduled event, add the action that you want to occur at your scheduled time. For this example, we will add two different actions in our scheduled event.
   
   Click the **+ Action** button to create a new event.
   
   Using the **Device** field, select the device that will take the action.
   <p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160602144712/ScheduleEvent-06.jpg" width="346" height="619" alt="Schedule Event"><br/><br/></p>
      
   After selecting the device for the action, use the **Action** field to choose what type of action will be triggered. The list of actions that you see displayed will always be appropriate based upon the device you selected for the action.
   
   <p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160602144827/ScheduleEvent-07.jpg" width="346" height="546" alt="Schedule Event"><br/><br/></p>

   Repeat the process for adding another device and action for this scheduled event.
   
   <p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160602144848/ScheduleEvent-08.jpg" width="346" height="546" alt="Schedule Event"><br/><br/></p>
   
7. You’re done. Click Save, and your Scheduled Event will be added to Cayenne. Cayenne will automatically take care of synchronizing with your devices and running the event at the appropriate time.

   <p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160602144957/Scheduling-MonthView.jpg" width="600" height="413" alt="Month View"></p>


### Scheduling views

You can view your scheduled events by Year, Month, Week or List View.

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160602145121/Scheduling-ListView.jpg" width="600" height="321" alt="Schedule List View"><br/></p>


### Receiving notifications

Cayenne can send you a notification when a scheduled event has occurred by email and/or text message.

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160602145334/ScheduleEvent-Notification.jpg" width="346" height="615" alt="Schedule Notifications"><br/></p>


## Rules Engine

### What is a trigger?

Cayenne allows you to create triggered actions on and between your Raspberry Pis, Arduinos, sensors and actuators based upon the state your devices. Simply put if a trigger event happens, then a resulting action happens.


### Setting up triggers

Let’s create our first trigger. We’ll create a trigger to turn on our light when the temperature reaches a certain value.

1. To begin creating a Trigger, click **Add New Trigger** from top right navigation.
   
   <p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160601122359/AddNew.jpg" width="260" height="252" alt="Add New Device"><br/></p>

2. The Create Trigger screen appears.
   
   <p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160602145622/Triggers-000.jpg" width="600" height="376" alt="Triggers"><br/></p>
   
   From here, you can fill in all the details required for creation of your trigger. When creating a new trigger, the empty screen serves as an overview of the creation process.

Example: **IF** my device senses something, **THEN** do something in response.

1. Let’s begin by giving our trigger a name. Enter **“Arduino Uno TMP36 is above 80, Turn on Raspberry Pi Light Switch”** into the Trigger Name field.

   <p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160602145732/Triggers-01.jpg" width="600" height="376" alt="Triggers"><br/><br/></p>

2. We’re going to trigger a light turning on when a temperature sensor on the Arduino device is above 80 degrees. The TMP36 temperature sensor is located on our Arduino device, so drag & drop the **Arduino** device into the **IF** statement.
   
   <p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160602145843/Triggers-02.jpg" width="600" height="376" alt="Triggers"><br/><br/></p>
   
3. After selecting the TMP36 temperature sensor, we can choose whether we want to trigger an action if temperature is above or below a certain value.

   We want to react to the temperature being high, so we select **Temperature** from the list and select **Temperature Above** in the options presented and choose 80 degrees for this example.
   
   <p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160602145950/Triggers-03.jpg" width="600" height="376" alt="Triggers"><br/><br/></p>
   
4. We want to take action once the temperature is high by turning on the light in our **Raspberry Pi*. Drag & drop the Raspberry Pi device into the **THEN** statement area.

   <p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160602150032/Triggers-04.jpg" width="600" height="376" alt="Triggers"><br/><br/></p>

5. We can now choose an action to take on our **Raspberry Pi**. Since we want to turn on the light, select **Light Switch** from the actions list and then choose On from the list of options available.

   <p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160602150131/Triggers-05.jpg" width="600" height="376" alt="Triggers"><br/><br/></p>

6. We’re done! Click **Save Trigger** to complete our trigger and return to the Triggers list where our new trigger is shown.

   <p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160602150219/Triggers-06.jpg" width="600" height="376" alt="Triggers"><br/><br/></p>
   
   Cayenne will will now start monitoring the temperature sensor and when it reaches the correct temperature your trigger will automatically run.
   
   
   
## Notification (Alerts)

### What is an alert?

Cayenne enables you to receive notifications when a device or sensor has reached a certain state. For example, you could be notified when a light gets turned on, a certain temperature is reached, or motion is detected.


### Setting up alerts

Let’s create our first notification alert. We’ll send a text message and email notification alert when the temperature outside reaches 90 degrees to send a text message and email.

1. To begin creating a Trigger Notification Alert, open the up the feature by selecting **Triggers** from **Add New navigation**.

   <p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160601122359/AddNew.jpg" width="260" height="252" alt="Add New Device"><br/></p>
   
2. The Create Trigger screen appears.
   
   <p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160602145622/Triggers-000.jpg" width="600" height="376" alt="Triggers"><br/><br/></p>
   
   From here, you can fill in all the details required for creation of your notification alert. To make this process easy, you will be guided through triggered alert creation that is easy to follow and select the devices and actions that you want.

**EXAMPLE:** **IF** my device senses something, **THEN** send me an alert notification

1. Let’s begin by giving our trigger a name. Enter **“Tmp36 is above 80, Send Notification”** into the Trigger Name field.
   
   <p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160602150757/Triggers-01-Notification.jpg" width="600" height="376" alt="Triggers"><br/><br/></p>

2. We’re going to trigger a notification alert when Tmp36 is above 80 degrees. The TMP36 temperature sensor is located on our Arduino device, so drag & drop the **Arduino** device into the **IF** statement.

   <p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160602150853/Triggers-02-Notification.jpg" width="600" height="376" alt="Triggers"><br/><br/></p>

3. After selecting the TMP36 temperature sensor, we can choose whether we want to trigger a notification if temperature is above or below a certain value.

   We want to react to the temperature being high, so we select **Temperature** from the list and select **Temperature Above** in the options presented and choose **80 degrees** for this example.
   
   <p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160602150957/Triggers-03-NOtification.jpg" width="600" height="376" alt="Triggers"><br/><br/></p>
   
4. We want to receive a triggered alert notification by text message and email each time TMP36 is above 80 degrees. Click **Setup notification**.

   <p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160602151034/Triggers-04-Notification.jpg" width="600" height="376" alt="Triggers"><br/><br/></p>
   
5. You can choose to receive notifications by text message and/or email. We want both, so we will choose **Select All**.   

   <p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160602151059/Triggers-05-Notification.jpg" width="600" height="376" alt="Triggers"><br/><br/></p>

6. Click **Add custom recipient** and enter in phone number to receive text. Then click **Add more recipients**? and add in the email address.

   <p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160602151114/Triggers-06-Notification.jpg" width="600" height="376" alt="Triggers"><br/><br/></p>   
   
7. We’re done! Click **Save Trigger** to complete our trigger alert and return to the Triggers list where our new trigger alert is shown.

   <p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160602151206/Triggers-07-Notification.jpg" width="600" height="376" alt="Triggers"><br/><br/></p>   
   
   Cayenne will will now start monitoring the temperature sensor and when it reaches the correct temperature a notification alert will be send by email and text message. <br/><br/>
   
 
### Receiving alerts
### SMS
### Email

