# Getting Started

## Create Cayenne Account
You can create an account from [Mobile](http://www.cayenne-mydevices.com/CayenneStaging/docs#mobile-apps) or online. Mobile is the easiest and fastest way, but instructions for online set up are below:

On the [Sign Up page](https://cayenne.mydevices.com/cayenne/signup?_ga=1.165612799.1524412540.1457034675), enter your Name, Email and create a Password.

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160601095407/Sign-Up.png" width="600" height="610" alt="Sign up for Cayenne"></p>


## Choose Device
Cayenne currently supports Raspberry Pi and Arduino devices currently.  Select the device you would like to get started with in your IoT project.

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160616132558/1st-Experience-Step-1-choose-device.png" width="600" height="384" alt="Choose a Device"></p>

The next section covers getting started with a Raspberry Pi device.  If you’re using an Arduino device to get started, [click here](http://www.cayenne-mydevices.com/CayenneStaging/docs#arduino-arduino).


## Raspberry Pi

### Getting started in minutes!
1. Power on your Raspberry Pi. Connect the power adapter to your Raspberry Pi.
2. Connect the Pi to the Internet. Connect your Raspberry Pi to the Internet using an Ethernet cable. Or, if you have a Wi-Fi dongle setup already this works too.
3. Make sure the Raspbian operating system is installed. Cayenne works with Jessie OS versions of Raspbian. Please make sure one of these is pre-installed to the sd card. If you need to install the Raspbian operating system, [click here](https://www.raspberrypi.org/downloads/raspbian/).

   **Note:** You do not need to make any configuration changes to the Pi device. Cayenne automatically handles setting up and configuring your Pi for use. However, it is recommended that you expand the filesystem on the flash card if necessary. Please refer to raspi-config if you need additional information on performing this step.

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160128155812/raspberry-pi-actual.png" width="600" height="610" alt="Raspberry Pi"></p>


### Installing Cayenne

**Installing from the Mobile App**

<p style="text-align:center"><iframe width="480" height="270" src="https://www.youtube.com/embed/J9zqvGWB5tM" frameborder="0" allowfullscreen></iframe></p>

Before you can manage your Raspberry Pi device using the mobile app, you must install the Cayenne app onto your mobile device. Installing and using the mobile app is the easiest way to get started with Cayenne. If you need additional help on this step, refer to the video tutorial above.

Visit the [Mobile App download page](http://www.cayenne-mydevices.com/CayenneStaging/docs#mobile-apps) to find the appropriate app store link for your device.

After installing the Cayenne app onto your mobile device, you will be guided through finding and installing Cayenne on all of your Raspberry Pi devices.

**Installing from the Web**

<p style="text-align:center"><iframe width="480" height="270" src="https://www.youtube.com/embed/Qx0IHv-UR-0" frameborder="0" allowfullscreen></iframe></p>

(1.) Before you can manage your Raspberry Pi device using the online dashboard, you must install Cayenne onto the device.

After verifying your Raspberry Pi is setup and powered on, you can continue with connecting your device to Cayenne.

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160616133028/1st-Experience-RPI-Step-2-setup-rpi.png" width="600" height="382" alt="Raspberry Pi Step 2"></p>

The instructions for installing Cayenne onto your device are displayed on screen. Follow the on screen instructions to start the installation process. If you need additional help on this step, refer to the video tutorial above.

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160616133821/1st-Experience-RPI-Step-3-connect-rpi.png" width="600" height="382" alt="Raspberry Pi Step 3"></p>

(2.) As soon as the installation process starts, the Installing screen automatically appears. From here you can check on the installation process as it completes.

Cayenne installs on your Raspberry Pi in 4 steps:

- **Step 1**: Installing libraries
- **Step 2**: Installing agent
- **Step 3**: Installing software
- **Step 4**: Installing drivers

__This may take up to 10 minutes. Please be patient.__

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160205134947/Screenshot-123.png" width="600" height="382" alt="Installing Cayenne"></p>

(3.) As soon as the installation process completes, the Online Dashboard will automatically appear. Your Raspberry Pi is now ready to use!

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160601102506/RaspberryPi-1stExperience.jpg" width="600" height="382" alt="Cayenne First Experience"></p>


### Sensors
Cayenne works with temperature, luminosity, pressure/distance, motion and generic sensors connected to your Raspberry Pi devices. [View supported sensors](http://www.cayenne-mydevices.com/CayenneStaging/docs#sensors-supported-hardware)

**EXAMPLE**: Let’s add a BMP180 temperature and pressure sensor to see how easy it is to get started.

Connect the BMP180 as shown here. [View BMP180 hardware tutorial](http://www.cayenne-mydevices.com/CayenneStaging/docs#rpi-bmp180)

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160601121157/RPI-BMP180-Step-4.png" width="600" height="193" alt="Cayenne Step 4"></p>


Click **Add New > Device / Widget**.

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160601122359/AddNew.jpg" width="260" height="252" alt="Add New Device"></p>

1. Select **Sensors, Temperature,** then **BMP180**.
2. Click **Add Sensor**.

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160617103039/Add-Device-RPI-BMP180.png" width="600" height="365" alt="Add Sensor"></p>


**Read your Sensor**

The BMP180 temperature and pressure widgets are added to your dashboard.

Let’s try it out! Place your hand on the BMP180 sensor. The temperature value updates as soon as a change in temperature is received.

You can check the current status of your sensor at any time by visiting the dashboard.

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160601122628/BMP180-RPIAdded.jpg" width="600" height="365" alt="Added Sensor"></p>


### Actuators
Cayenne works with light, motor, valve, relay and generic actuators that are connected to your Raspberry Pi devices. [View supported actuators](http://www.cayenne-mydevices.com/CayenneStaging/docs#actuators-supported-hardware)

**EXAMPLE**: We will switch on an LED connected to your Raspberry Pi using Cayenne.

Connect an LED to Channel 23 as shown here. [View LED tutorial](http://www.cayenne-mydevices.com/CayenneStaging/docs#rpi-digital-output-led)

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160601121207/RPI-Digital-Out-Led-Step-2.png" width="600" height="193" alt="LED Step 2"></p>

Click **Add New > Device / Widget**.


<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160601122359/AddNew.jpg" width="260" height="252" alt="Add New Device"></p>

1. Select **Actuators**, then **Light**, then **Light Switch**.
2. Enter “LED” in name field.
3. Choose channel 23.
4. Click **Add Actuator**.


<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160617103241/Add-Device-RPI-Lightswitch.jpg" width="600" height="365" alt="Light Switch"></p>

The LED widget has been added to your dashboard. Click the LED button in the dashboard to turn the LED on and off.

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160601123646/LightSwitch-RPI-todashboard.jpg" width="600" height="365" alt="Light Switch to Dashboard"></p>


### Extensions

You can add analog, digital and PWM extensions to your Raspberry Pi. This allows you to add more sensors and actuators to your Raspberry Pi. [View supported extensions](http://www.cayenne-mydevices.com/CayenneStaging/docs#extensions-supported-hardware)

## Arduino

### Getting started in minutes!
<p style="text-align:center"><iframe width="480" height="270" src="https://www.youtube.com/embed/hmIGRrvevCA" frameborder="0" allowfullscreen></iframe></p>

Before you can manage your Arduino device using the online dashboard, you must setup your device and install the Cayenne Arduino Library onto the device.

### Arduino Setup

Begin by verifying that your Arduino board and PC/Mac are correctly set up before continuing.

1. **Make sure your Arduino is connected to the Internet**<br/>
   On most Arduino boards, you will need to connect an Ethernet or Wi-Fi shield in order to connect your board to the Internet. Verify that you have a shield supported by Cayenne installed and working
   
2. **Make sure your Arduino is connected to a PC/Mac via the USB cable**<br/>
   Power on your Arduino by connecting your Arduino with a USB cable (or FTDI connector if you’re using an Arduino pro). You should see the power LED lit on your board.
   
<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160616134313/1st-Experience-Arduino-Step-2-setup-arduino.png" width="600" height="384" alt="Step 2 Arduino"></p>


#### Using Cayenne Arduino Library
The Cayenne Arduino Library is a collection of code, known as sketch files, that makes it easy for you to connect and send data to and from sensors, actuators and devices connected to Arduino boards. Cayenne sketch files can be combined with other sketch files for your IoT projects.

If you need to download the Cayenne Arduino Library, [click here](https://s3.amazonaws.com/mydevices-cayenne/arduino/lib/prod/Cayenne.zip).


##### Installing Arduino IDE Software
To use the Cayenne Arduino Library, the Arduino IDE software should be installed. Go to [https://www.arduino.cc/en/Main/Software](https://www.arduino.cc/en/Main/Software) to download and install the Arduino IDE software if you need it. Arduino IDE can be installed on Windows, Mac or Linux computers.


##### Installing Cayenne Library

The Cayenne Arduino Library is distributed as a ZIP file. Do not unzip the downloaded library, leave it as is. Open the Arduino IDE and navigate to **Sketch > Include Library**. At the top of the drop down list, select the option **Add .ZIP Library**.

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160601124500/ImportingCayenneLibrary.jpg" width="600" height="913" alt="Importing Cayenne Library"></p>

You will be prompted to select the library you would like to add. Navigate to where you downloaded the Cayenne library zip file and select the **Cayenne.zip** file.

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160601124529/CayenneZipFile.jpg" width="600" height="498" alt="Cayenne ZIP File"></p>

The Cayenne zip file has now been expanded in the libraries folder in your Arduino sketches directory.

Return to the **Sketch > Include Library** menu. You should now see the **Cayenne** library at the bottom of the drop-down menu under **Contributed Libraries**. The Cayenne library is now ready to be used in your sketch file.

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160601124601/CayenneLibraryInstalled.jpg" width="600" height="925" alt="Cayenne Library Installed"></p>


#### Connect your Arduino

After setting up your PC/Mac computer with the Arduino IDE and the Cayenne Library, you are ready to install Cayenne onto your device. Continue to Step 3 of the Arduino installation, where you will connect your board with Cayenne.

On this screen, select the Arduino board that you are using from the list of [supported boards](http://www.cayenne-mydevices.com/CayenneStaging/docs#arduino-microcontrollers). As you select your Arduino board, a list of connections appears below the board name. Select the connection type that you are using.

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160616135653/1st-Experience-Arduino-Step-3-board-expanded1.png" width="600" height="385" alt="Arduino Step 3"></p>

Click on the Sketch button next to the connection you will be using and a popup will appear with the sketch file you will need when flashing your Arduino device. The sketch file will contain everything you need to connect your device to Cayenne, including your [authentication token](http://www.cayenne-mydevices.com/CayenneStaging/docs#finding-auth-token).

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160616135934/1st-Experience-Arduino-Step-3-connection-example.png" width="600" height="385" alt="Arduino Step 3 Connection Example"></p>

Copy & paste the sketch file contents into Arduino IDE and select **Sketch -> Upload** to upload the sketch file to your device.

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160616151042/Arduino-IDE-paste-example-sketch-for-connection.png" width="600" height="555" alt="Arduino IDE paste example sketch"></p>

As soon as your Arduino device comes online and connects to Cayenne, you will see your Arduino Board in the online dashboard.

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160601125316/Arduino1stExperience.png" width="600" height="385" alt="Arduino 1st Experience"></p>

**Congrats! You are all set! Now your hardware is connected to the Cayenne Cloud!**

If you run into any troubles, see Troubleshooting for things to check.

### Sensors

Cayenne works with any sensor that is connected to an Arduino. We’ve created [sketch files](https://github.com/myDevicesIoT/CayenneArduinoSamples) for the various temperature, luminosity, pressure, proximity, motion and generic sensor models.

**EXAMPLE:** Let’s add temperature sensor TMP36 to see how easy it is.

Connect the TMP36 as shown here. [View TMP36 hardware tutorial](http://www.cayenne-mydevices.com/CayenneStaging/docs#arduino-tmp36)

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160601121144/Arduino_TMP36_step3_bb.png" width="600" height="380" alt="Arduino TMP36 Step 3"></p>

Click **Add New > Device / Widget**.

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160601122359/AddNew.jpg" width="260" height="252" alt="Add New Device"></p>

1. Choose **Sensor > Temperature > TMP36**.
2. Choose **Virtual** from the I/O field.
3. We will use Virtual Pin 1 for this example. Choose **V1** from the **Pin** field.
4. Click the **Step 1: Sketch File** button to view the sketch file.

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160617103706/Add-Device-Arduino-TMP361.png" width="600" height="365" alt="Arduino Add Device TMP361"></p>

A popup will appear showing the TMP36 sketch file. Copy the sketch file contents to the clipboard and open Arduino IDE.

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160617151040/Add-Device-Arduino-TMP36-Sketch-file2.png" width="600" height="386" alt="Arduino Add Device TMP361 Sketch File"></p>

Paste the TMP36 sketch file code into the Arduino IDE. After copying & pasting the example sketch files, you will want to double check that your **authentication token** is correct as well as update any pin assignments that appear in the sketch file. [Read more about using sketch files](http://www.cayenne-mydevices.com/CayenneStaging/docs#using-sketch-files-arduino)

In this case, we are using the default Virtual Pin 1 which is already defined in the sketch file, so the sketch file should be OK to use as is. After verifying the sketch file looks good, select **Sketch -> Upload** to upload the sketch file to your device.

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160603151539/TMP36-ArduinoIDE.jpg" width="600" height="836" alt="Arduino IDE TMP361"></p>

In the Cayenne dashboard, you can now click the **Step 2: Add Sensor** button and the TMP36 widget will be added to your dashboard. You can change widget type and settings by clicking on the cogwheel icon in the top right corner of the TMP36 widget.

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160601131032/Arduino-TMP36.jpg" width="600" height="336" alt="Arduino IDE TMP361"></p>

### Actuators

Cayenne works with actuators that are connected to an Arduino.  We’ve created [sketch files](https://github.com/myDevicesIoT/CayenneArduinoSamples/tree/master/Actuators) for light, motor, valve, relay and generic actuators.

**EXAMPLE:** Let’s add a luminosity actuator widget.

For this example, attach a LED to a PWM-enabled Pin on your Arduino Uno. Let’s use D6 in this example. [View Luminosity hardware tutorial](http://www.cayenne-mydevices.com/CayenneStaging/docs#arduino-luminosity)

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160601112652/Arduino-Luminosity-Step-2.png" width="600" height="307" alt="Arduino Luminosity Step 2"></p>

Click **Add New > Device / Widget**.

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160601122359/AddNew.jpg" width="260" height="252" alt="Add New Device"></p>

1. Choose **Actuator > Light > Luminosity**.
2. Choose **Virtual** from the I/O field.
3. We will use Virtual Pin 1 for this example. Choose **V1** from the **Pin field**.
4. Click the **Step 1: Sketch File** button to view the sketch file.

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160617110431/Add-Device-Arduino-Luminosity.png" width="600" height="364" alt="Arduino Luminosity Add Device"></p>

A popup will appear showing the Luminosity sketch file. Copy the sketch file contents to the clipboard and open Arduino IDE.

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160617152613/Add-Device-Arduino-Luminosity-sketch-file2.png" width="600" height="386" alt="Arduino Luminosity Sketch File"></p>

Paste the Luminosity sketch file code into the Arduino IDE. After copying & pasting the example sketch files, you will want to double check that your **authentication token** is correct as well as update any pin assignments that appear in the sketch file. [Read more about using sketch files](http://www.cayenne-mydevices.com/CayenneStaging/docs#using-sketch-files-arduino)

In this case, the example sketch file assumes that we used Digital Pin 3 to connect our Luminosity actuator, but we used Digital Pin 6 instead. We will need to update the sketch file to correct the pin. Find and update the **LED_DIGITAL_PIN** definition so that it points at pin 6.

```
#define LED_DIGITAL_PIN 6
```

After verifying the sketch file looks good, select Sketch -> Upload to upload the sketch file to your device.

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160617151924/Arduino-Luminosity-in-Arduino-IDE.png" width="600" height="554" alt="Arduino Luminosity in Arduino IDE"></p>

In the Cayenne dashboard, you can now click the **Step 2: Add Actuator** button and the luminosity widget will be added to your dashboard. You can now use the slider to control the brightness of the LED.

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160601131732/Arduino1stExperience-Luminosity.jpg" width="600" height="376" alt="Arduino Luminosity"></p>

### Add custom widgets

We’ve integrated some specific sensors and actuators, but there are thousands of sensors, actuators and other devices that get connected to Arduino boards. Custom widgets allow you to send and receive data from any device that is connected to your Arduino board to Cayenne.

[Cayenne Custom Widgets Documentation](http://www.cayenne-mydevices.com/CayenneStaging/docs#widgets)

**EXAMPLE:** Let’s see how easy it is to use a Custom Widget in Cayenne. We will switch on an LED connected to your Raspberry Pi using a custom Button widget.

Connect an LED to Digital Pin 8 as shown here. [View light switch tutorial](http://www.cayenne-mydevices.com/CayenneStaging/docs#arduino-light-switch)

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160601105118/Arduino_LED_step2_bb.png" width="600" height="317" alt="Arduino LED Step 2"></p>

Click **Add New > Device / Widget**.

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160601122359/AddNew.jpg" width="260" height="252" alt="Add New Device"></p>

1. Select **Custom Widgets**, then the **Button** Widget.
2. Enter the following settings:<br/>
   **Widget Name:** LED<br/>
   **Device:** Arduino<br/>
   **Connectivity:** Digital<br/>
   **Pin:** D8<br/>
   **Icon:** LED
3. Click **Add Widget**.

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160601132656/Arduino-Custom-Button-Widget.png" width="600" height="355" alt="Arduino Custom Button Widget"></p>

The button widget gets added to your dashboard.

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160601132737/Arduino1stExperience-AddLED.jpg" width="600" height="336" alt="Arduino Add LED"></p>

Push the button in your online dashboard to turn the LED on and off. You’re now ready to start using Cayenne for your IoT projects.

Check out other example sketches at our [Cayenne Github](https://github.com/myDevicesIoT/CayenneArduinoSamples). Feel free to experiment and combine different examples together to create your own amazing projects.


### Troubleshooting

If you don’t see your Arduino device connected to Cayenne, or if you’re running into trouble successfully programming your Arduino with the Arduino IDE, here are a few things to check.


1. **Make sure your Arduino is connected to the Internet**<br/>
   On most Arduino boards, you will need to connect an Ethernet or Wi-Fi shield in order to connect your board to the Internet. Verify that you have [a shield supported by Cayenne](http://www.cayenne-mydevices.com/CayenneStaging/docs#arduino-shields-connections) installed and working.<br/><br/>
2. **Make sure your Arduino is connected to a PC/Mac via the USB cable**<br/>
   Power on your Arduino by connecting your Arduino with a USB cable (or FTDI connector if you’re using an Arduino pro). You should see the power LED lit on your board.<br/><br/>
3. **Configure the Arduino IDE**<br/>
   First, verify that you have the [Arduino IDE](https://www.arduino.cc/en/Main/Software) installed.
   Open the Arduino IDE program and verify that the correct **Board** is selected.
   <p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160616113931/Arduino-IDE-board-selection.png" width="600" height="501" alt="Arduino IDE Board Selection"></p>
   Next, verify that you have the correct **Port** selected for communicating with your Arduino. Pick the correct port based upon how you are connecting your Arduino to your PC/Mac.
   <p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160616114005/Arduino-IDE-port-selection.png" width="600" height="501" alt="Arduino IDE Port Selection"></p>
4. **Verify that you have the Cayenne Library installed**<br/>
   Verify that you see the Cayenne library installed under **File -> Examples -> Cayenne**. If you do not, [download the library](https://s3.amazonaws.com/mydevices-cayenne/arduino/lib/prod/Cayenne.zip) and include it into the Arduino IDE. For more help on this, see [Installing Cayenne Library into your Arduino IDE](http://www.cayenne-mydevices.com/CayenneStaging/docs#installing-library-arduino-ide).   
   <p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160616115052/Arduino-IDE-Cayenne-lib-installed.png" width="600" height="555" alt="Arduino IDE Library Installed"></p>
5. **Verify that your Arduino is connected with Cayenne**<br/>   
   You can use the Serial Monitor tool in the Arduino IDE to view some connection information. After uploading your sketch file to the Arduino device, open the **Serial Monitor** and look for the Cayenne connection.   
   <p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160616114750/Arduino-Serial-Monitor-option.png" width="600" height="487" alt="Arduino Serial Monitor"></p>
   In the output of the Serial Monitor, you should see something like this:
   ```
   Getting IP...
   My IP: 192.168.0.10
   Connecting to arduino.mydevices.com:8442
   Ready (ping: 109ms).
   ```
   If you don’t, this means your board is not connected to the Internet to send data to the Cayenne cloud. You will need to verify that your Arduino is connected to the Internet.
   
   If you don’t see any outptut in the Serial Monitor, leave it open and Reset your Arduino board.
