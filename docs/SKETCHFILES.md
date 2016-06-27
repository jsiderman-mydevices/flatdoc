# Sketch Files

## About
Programs written using Arduino Software IDE for installing on Arduino and similar microcontrollers are called sketch files. These sketches are written in the text editor and are saved with the file extension .ino. The editor has features for cutting/pasting and for searching/replacing text. The message area gives feedback while saving and exporting and also displays errors. The console displays text output by the Arduino Software (IDE), including complete error messages and other information. The bottom righthand corner of the window displays the configured board and serial port. The toolbar buttons allow you to verify and upload programs, create, open, and save sketches, and open the serial monitor.

[Learn more about writing Sketch files](https://www.arduino.cc/en/Guide/Environment#toc1)


## Cayenne Arduino Library
The Cayenne Arduino library is a collection of example sketch files and libraries for connecting and sending data to and from your Arduino hardware.   [View Cayenne Arduino Library](https://github.com/myDevicesIoT/CayenneArduinoSamples)


## Using Sketch Files
Cayenne sketch files will help you get your hardware online quickly, adding sensors, actuators, custom widgets and using major features. You can access the Cayenne sketch files from a few different ways. 

**Through the Cayenne dashboard**

The easiest way to get the sketch files you need is to use the **Sketch File** button found when adding your widget from the Cayenne dashboard. When you open the sketch file from the dashboard, Cayenne will create a personalized version of the sketch file just for you; automatically filling in details such as your **authentication token** and some of the Pin values based upon fields you selected on screen.

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160617151040/Add-Device-Arduino-TMP36-Sketch-file2.png" width="300" height="386" alt="Using Sketch Files"><br/><br/></p>

**Through Cayenne GitHub**

You can find and browse the complete list of example sketch files located on the [Cayenne GitHub](https://github.com/myDevicesIoT/CayenneArduinoSamples).

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160617160351/Github-root.png" width="600" height="300" alt="Using Sketch Files"><br/><br/></p>

**Through Arduino IDE**

After adding the Cayenne library to Arduino IDE, you can open example Cayenne sketch files from the **File -> Examples** menu.

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160601124630/CayenneExampleSketchFiles.jpg" width="600" height="587" alt="Using Sketch Files"><br/><br/></p>


### Customizing Sketch Files

After locating the example sketch file that you need for your Arduino board or connected device, you will need to copy & paste the content into the Arduino IDE. After copying & pasting the example sketch files, you will want to double check that the content of the sketch file is correct.

**Verify your authentication token**

The authentication token is the unique identifier that connects your Arduino board to the Cayenne Cloud and enables interactions to and from Cayenne and your hardware.  An Auth token is generated each time you add a new Arduino board.

If you use an example sketch file from Cayenne, you will want to make sure that your authentication token is present. To verify this, check for the following line in your sketch file:
 
```
char token[] = "AuthenticationToken";
```
 
Make sure to update this line in the sketch file to include your Arduino board’s unique authentication token. It should look similar to this:

```
char token[] = "a5cpbk9k1w";
```

If you need help, refer to [Finding your authentication token](http://www.cayenne-mydevices.com/CayenneStaging/docs/#finding-auth-token).<br/><br/>



**Verify pin assignments**

Many sketch files will include default pin assignments for those pins used when reading/writing to the device. If you have connected your device in a different manner than mentioned in the example, you will need to customize these lines. You will find helpful information on using the example file within each sketch file.
 
For example, let’s look at the [**Luminosity** sketch file](https://github.com/myDevicesIoT/CayenneArduinoSamples/blob/master/Actuators/Luminosity/Luminosity.ino). The sketch file begings with the following code:

```
#define CAYENNE_PRINT Serial // Comment this out to disable prints and save space
#include <CayenneEthernet.h>
#define LED_VIRTUAL_PIN 1
#define LED_DIGITAL_PIN 3
```

The code assumes that you have your actuator connected to the Arduino’s **Digital Pin 3**. It also assumes that you will be using **Virtual Pin 1** when adding the Luminosity widget in the Cayenne dashboard.

Let’s assume that you didn’t attach your Luminosity actuator to Digital Pin 3, but instead you used **Digital Pin 6**. You will need to update the sketch file to correct the pin. Update the **LED_DIGITAL_PIN** definition so that it points at pin 6.

```
#define LED_DIGITAL_PIN 6
```

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160617151924/Arduino-Luminosity-in-Arduino-IDE.png" width="600" height="554" alt="Using Sketch Files"><br/><br/></p>

Once you’ve looked over your sketch file and updated all values, use **Sketch -> Upload** in Arduino IDE to upload the sketch file to your device.


### Combining Sketch Files

## Finding Auth Token

If you ever need to find your Auth Token again, click on the **cogwheel icon** next to your Arduino board name and click **Configure**.

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160601130027/Configure.jpg" width="232" height="184" alt="Finding Auth Token"><br/><br/></p>

Your Auth Token can be found on this settings screen.

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160601130044/ArduinoConfigure-e1464901755145.jpg" width="600" height="340" alt="Finding Auth Token"><br/><br/></p>


## Code examples (Sketch)

**[Actuators](https://github.com/myDevicesIoT/CayenneArduinoSamples/tree/master/Actuators)**

* [GenericDigitalOutput](https://github.com/myDevicesIoT/CayenneArduinoSamples/blob/master/Actuators/GenericDigitalOutput/GenericDigitalOutput.ino)
* [GenericPWMOutput](https://github.com/myDevicesIoT/CayenneArduinoSamples/blob/master/Actuators/GenericPWMOutput/GenericPWMOutput.ino)
* [LightSwitch](https://github.com/myDevicesIoT/CayenneArduinoSamples/blob/master/Actuators/LightSwitch/LightSwitch.ino)
* [Luminosity](https://github.com/myDevicesIoT/CayenneArduinoSamples/blob/master/Actuators/Luminosity/Luminosity.ino)
* [MotorSwitch](https://github.com/myDevicesIoT/CayenneArduinoSamples/blob/master/Actuators/MotorSwitch/MotorSwitch.ino)
* [RelaySwitch](https://github.com/myDevicesIoT/CayenneArduinoSamples/blob/master/Actuators/RelaySwitch/RelaySwitch.ino)
* [ServoMotor](https://github.com/myDevicesIoT/CayenneArduinoSamples/blob/master/Actuators/ServoMotor/ServoMotor.ino)
* [ValveSwitch](https://github.com/myDevicesIoT/CayenneArduinoSamples/blob/master/Actuators/ValveSwitch/ValveSwitch.ino)
<br/><br/>

**[Basics](https://github.com/myDevicesIoT/CayenneArduinoSamples/tree/master/Basics)**

* [ReceiveData](https://github.com/myDevicesIoT/CayenneArduinoSamples/blob/master/Basics/ReceiveData/ReceiveData.ino)
* [SendData](https://github.com/myDevicesIoT/CayenneArduinoSamples/blob/master/Basics/SendData/SendData.ino)
* [SendDataOnRequest](https://github.com/myDevicesIoT/CayenneArduinoSamples/blob/master/Basics/SendDataOnRequest/SendDataOnRequest.ino)
* [SyncAll](https://github.com/myDevicesIoT/CayenneArduinoSamples/blob/master/Basics/SyncAll/SyncAll.ino)
* [SyncData](https://github.com/myDevicesIoT/CayenneArduinoSamples/blob/master/Basics/SyncData/SyncData.ino)
<br/><br/>

**[Connections](https://github.com/myDevicesIoT/CayenneArduinoSamples/tree/master/Connections)**

* [ArduinoEthernet](https://github.com/myDevicesIoT/CayenneArduinoSamples/blob/master/Connections/ArduinoEthernet/ArduinoEthernet.ino)
* [ArduinoEthernetManual](https://github.com/myDevicesIoT/CayenneArduinoSamples/blob/master/Connections/ArduinoEthernetManual/ArduinoEthernetManual.ino)
* [ArduinoEthernetW5200](https://github.com/myDevicesIoT/CayenneArduinoSamples/blob/master/Connections/ArduinoEthernetW5200/ArduinoEthernetW5200.ino)
* [ArduinoEthernetW5500](https://github.com/myDevicesIoT/CayenneArduinoSamples/blob/master/Connections/ArduinoEthernetW5500/ArduinoEthernetW5500.ino)
* [ArduinoSerialUSB](https://github.com/myDevicesIoT/CayenneArduinoSamples/blob/master/Connections/ArduinoSerialUSB/ArduinoSerialUSB.ino)
* [ArduinoWiFi](https://github.com/myDevicesIoT/CayenneArduinoSamples/blob/master/Connections/ArduinoWiFi/ArduinoWiFi.ino)
* [ArduinoWiFi101](https://github.com/myDevicesIoT/CayenneArduinoSamples/blob/master/Connections/ArduinoWiFi101/ArduinoWiFi101.ino)
* [ArduinoYun](https://github.com/myDevicesIoT/CayenneArduinoSamples/blob/master/Connections/ArduinoYun/ArduinoYun.ino)
<br/><br/>

**[Custom Widgets](https://github.com/myDevicesIoT/CayenneArduinoSamples/tree/master/CustomWidgets)**

* [2StateWidget](https://github.com/myDevicesIoT/CayenneArduinoSamples/blob/master/CustomWidgets/TwoStateWidget/TwoStateWidget.ino)
* [ButtonWidget](https://github.com/myDevicesIoT/CayenneArduinoSamples/blob/master/CustomWidgets/ButtonWidget/ButtonWidget.ino)
* [GaugeWidget](https://github.com/myDevicesIoT/CayenneArduinoSamples/blob/master/CustomWidgets/GaugeWidget/GaugeWidget.ino)
* [LineChartWidget](https://github.com/myDevicesIoT/CayenneArduinoSamples/blob/master/CustomWidgets/LineChartWidget/LineChartWidget.ino)
* [SliderWidget](https://github.com/myDevicesIoT/CayenneArduinoSamples/blob/master/CustomWidgets/SliderWidget/SliderWidget.ino)
* [ValueWidget](https://github.com/myDevicesIoT/CayenneArduinoSamples/blob/master/CustomWidgets/ValueWidget/ValueWidget.ino)
<br/><br/>

**[Sensors](https://github.com/myDevicesIoT/CayenneArduinoSamples/tree/master/Sensors)**

* [AnalogDistanceSensor](https://github.com/myDevicesIoT/CayenneArduinoSamples/blob/master/Sensors/AnalogDistanceSensor/AnalogDistanceSensor.ino)
* [AnalogLoadPressureSensor](https://github.com/myDevicesIoT/CayenneArduinoSamples/blob/master/Sensors/AnalogLoadPressureSensor/AnalogLoadPressureSensor.ino)
* [BMP180](https://github.com/myDevicesIoT/CayenneArduinoSamples/blob/master/Sensors/BMP180/BMP180.ino)
* [DS18B20](https://github.com/myDevicesIoT/CayenneArduinoSamples/blob/master/Sensors/DS18B20/DS18B20.ino)
* [DigitalMotionSensor](https://github.com/myDevicesIoT/CayenneArduinoSamples/blob/master/Sensors/DigitalMotionSensor/DigitalMotionSensor.ino)
* [GenericAnalogInput](https://github.com/myDevicesIoT/CayenneArduinoSamples/blob/master/Sensors/GenericAnalogInput/GenericAnalogInput.ino)
* [GenericDigitalInput](https://github.com/myDevicesIoT/CayenneArduinoSamples/blob/master/Sensors/GenericDigitalInput/GenericDigitalInput.ino)
* [Photoresistor](https://github.com/myDevicesIoT/CayenneArduinoSamples/blob/master/Sensors/Photoresistor/Photoresistor.ino)
* [TMP102](https://github.com/myDevicesIoT/CayenneArduinoSamples/blob/master/Sensors/TMP102/TMP102.ino)
* [TMP36](https://github.com/myDevicesIoT/CayenneArduinoSamples/blob/master/Sensors/TMP36/TMP36.ino)
* [TSL2561](https://github.com/myDevicesIoT/CayenneArduinoSamples/blob/master/Sensors/TSL2561/TSL2561.ino)
* [Thermistor](https://github.com/myDevicesIoT/CayenneArduinoSamples/blob/master/Sensors/Thermistor/Thermistor.ino)
* [VCNL4000](https://github.com/myDevicesIoT/CayenneArduinoSamples/blob/master/Sensors/VCNL4000/VCNL4000.ino)


## Using Analog vs. Virtual pins

**Arduino analog data** <br/>
When reading Analog devices with the Arduino microcontroller, the Arduino’s built in analog to digital converter (ADC) will be used. The value returned by the ADC is a 10-bit value (0 – 1023) that is proportional to the amount of voltage being applied to the pin. It is important to keep this in mind when examining the data returned by your device. For example, if you connect a Temperature sensor to an analog pin, it will not automatically return a temperature reading as you may expect. Instead, additional formulas would be needed to convert the voltage reading returned from the ADC into meaningful temperature data for the sensor.

**NOTE:** If you use Cayenne’s built-in library of devices, this conversion can be performed automatically!
[View list of supported sensors](http://www.cayenne-mydevices.com/CayenneStaging/docs/#sensors-supported-hardware)

**Arduino Virtual pins** <br/>
If you wish convert your analog reading to a more meaningful data point, or you wish to change the way your data is formatted, you can instead use a Virtual pin.

Using a Virtual pin, you have complete control over the data is returned to Cayenne. You can apply whatever formatting or data conversions are needed and when viewing the data in Cayenne, it will be in the exact format that you’ve specified. For example, you can perform an Analog read of your temperature sensor, convert the data to a Temperature value in Celsius, and return the data to Cayenne. Now when you view your sensor in Cayenne, you will see Temperature data reported exactly as you expected.

In order to use Virtual pins, you will need to include some code in your sketch file to handle reading and formatting for your sensor. Cayenne makes this easy by providing various example sketch files and information that you can use to get started.
[View sketch file information](http://www.cayenne-mydevices.com/CayenneStaging/docs/#code-examples-sketch)


## Virtual Pins

Virtual pins are different than Digital and Analog Input/Output (I/O) pins. Cayenne lets you control any hardware connected to Digital and Analog pins without having to write any additional code.

Virtual pins enable some very powerful customizations for your IoT projects because they allow you to interface with any device library. We use Virtual pins to display and send any data from your microcontroller to the Cayenne web dashboard and (coming soon) mobile apps. You can think about Virtual pins as channels for sending various types of data from your microcontroller to Cayenne. Remember, Virtual pins have no physical properties.

## Virtual Pin Data Types

Currently, Cayenne supports sending data as an integer or float format. We plan to support additional data types such as strings and arrays in the future.

**Cayenne.virtualWrite(vPin, value)**<br/>
You can send various formats of data to Virtual Pins

Send an integer value to a virtual pin:

```
Cayenne.virtualWrite(V1, 123)
```
<br/>

Send a float value to a virtual pin:<br/>
```
Cayenne.virtualWrite(V1, 12.34)
```
<br/>

**CAYENNE_IN(vPIN)**
CAYENNE_IN defines a function that is called when the device receives an updated Virtual pin value from the Cayenne server.

```
CAYENNE_IN(V1)
{
int value = getValue.asInt(); // Get value as integer
}
``` 
<br/>

**CAYENNE_OUT(vPIN)**
CAYENNE_OUT defines a function that is called when the device is request to send it’s current value of Virtual pin to the Cayenne server. Normally, this function contains some Cayenne.virtualWrite calls.

```
CAYENNE_OUT(V1)
{
Cayenne.virtualWrite(V1, newValue);
}
```
<br/>

**CAYENNE_CONNECTED()**
This function is called every time Cayenne connects to the server. It’s convenient to call sync functions here.

```
CAYENNE_CONNECTED() {
// Your code here
}
``` 
<br/>

**Cayenne.syncAll()**
Request the Cayenne server to send the most recent values for all widgets. All analog/digital pin states will be restored and every virtual pin will generate CAYENNE_IN event.

```
CAYENNE_CONNECTED() {
  if (isFirstConnect) {
   Cayenne.syncAll();
 }
}
``` 
<br/>

**Cayenne.syncVirtual(vPin)**
Requests a single virtual pin value update. The corresponding CAYENNE_IN handler is called as a result.

```
Cayenne.syncVirtual(V1);
```
<br/>

## Using IDE

To use Cayenne’s library of sketch files, we recommend using Arduino IDE or similar IDE for installing on your Arduinio hardware. [View installing Cayenne Arduino Library](http://www.cayenne-mydevices.com/CayenneStaging/resources/docs/installing-library-arduino-ide/)






