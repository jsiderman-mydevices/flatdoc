# Custom Widgets

There are 3 types of Widgets:

1. **Control**: Send commands to a device or sensor. You use them to control your devices or sensors.
   - [Button](http://www.cayenne-mydevices.com/CayenneStaging/docs/#button-control)
   - [Slider](http://www.cayenne-mydevices.com/CayenneStaging/docs/#slider-control)
2. **Data Display**: Used for visualization of data that comes from your connected devices or sensors.
   - [Line Chart](http://www.cayenne-mydevices.com/CayenneStaging/docs/#line-chart-display)
   - [Value](http://www.cayenne-mydevices.com/CayenneStaging/docs/#value-display)
   - [Gauge](http://www.cayenne-mydevices.com/CayenneStaging/docs/#gauge-display)
   - [2 State](http://www.cayenne-mydevices.com/CayenneStaging/docs/#2-state-display)

   

## Control

### Button

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160601104330/widget-tutorial-button-header.png" width="346" height="124" alt="Widget Tutorial"><br/><br/></p>

Send values like LOW/HIGH and On/Off to change state. An optional icon can be shown in the button widget.

**Example States**

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160602092259/Widget-Button.jpg" width="600" height="173" alt="Widget Button"><br/><br/></p>


#### Button Arduino Tutorial

This tutorial explains how to use the Button controller widget to add an actuator connected to your Arduino.

Let’s look at each dropdown field that will be used when adding your actuator.

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160511022536/widget-tutorial-button-form.png" width="346" height="490" alt="Widget Tutorial Form"><br/><br/></p>

**Name** <br/>
Give your actuator a name. 

**Device** <br/>
Select your Arduino device.

**Connectivity** <br/>
Select your method of connectivity; will the button widget be connected to a digital pin on the Arduino, or will it make use of the Cayenne virtual pins?

   - **Digital** <br/>
You can control the actuator state (high / low) through the digital pin on the Arduino.

   - **Virtual** <br/>
[Virtual pins](http://www.cayenne-mydevices.com/CayenneStaging/docs/#virtual-pins-microcontrollers) are channels to send and receive different data types from and to the Arduino (e.g. SPI, I2C, 1-Wire and devices connected to Arduino expansion boards). There are 26 virtual pins available for each Arduino board.

**Data, Unit, Icon** <br/>
Select the Data type, the Units, and the Icon to be used for the widget. For example, a temperature sensor could have a Data type of temperature, Units of Celsius, and a thermometer Icon.

**Add Widget** <br/>
After filling in each of the fields for your widget, click **Add Widget** and the widget will be added to your dashboard.

**Sketch File** <br/>
[Arduino Button Widget sketch file](https://github.com/myDevicesIoT/CayenneArduinoSamples/blob/master/CustomWidgets/ButtonWidget/ButtonWidget.ino)


### Slider

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160601104436/widget-tutorial-slider-header.png" width="346" height="124" alt="Slider Tutorial"><br/><br/></p>

Change the value of the connected device, such as dimming a light. The units, MIN and MAX values can be adjusted in settings.

**Example States**

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160602103206/Widget-Slider.jpg" width="600" height="147" alt="Slider Widget"><br/><br/></p>


#### Slider Arduino Tutorial

This tutorial explains how to use the Slider widget to add an actuator connected to your Arduino.

Let’s look at each dropdown field that will be used when adding your actuator.

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160512062826/widget-tutorial-slider-form.png" width="346" height="535" alt="Slider Tutorial Form"><br/><br/></p>

**Name** <br/>
Give your actuator a name. 

**Device** <br/>
Select your Arduino device.

**Connectivity** <br/>
Select your method of connectivity; will the slider widget use the physical PWM pins on the Arduino, or will it make use of the Cayenne virtual pins?

   - **Digital** <br/>
The Arduino may have several pins that can be used as PWM outputs (e.g. Arduino Uno has D3, D5, D6, D9, D10 & D11).

   - **Virtual** <br/>
[Virtual pins](http://www.cayenne-mydevices.com/CayenneStaging/docs/#virtual-pins-microcontrollers) are channels to send and receive different data types from and to the Arduino (e.g. SPI, I2C, 1-Wire and devices connected to Arduino expansion boards). There are 26 virtual pins available for each Arduino board.
**Data, Unit, Icon** <br/>
Select the Data type, the Units, and the Icon to be used for the widget. For example, a temperature sensor could have a Data type of temperature, Units of Celsius, and a thermometer Icon.

**Add Widget** <br/>
After filling in each of the fields for your widget, click **Add Widget** and the widget will be added to your dashboard.

**Sketch File** <br/>
[Arduino Slider Widget sketch file](https://github.com/myDevicesIoT/CayenneArduinoSamples/blob/master/CustomWidgets/SliderWidget/SliderWidget.ino)


## Data Display

### Line Chart

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160601104333/widget-tutorial-linechart-header.png" width="346" height="124" alt="Line Chart Tutorial"><br/></p>

Displays live or historical data from the attached device. Historical data can be filtered by minute, hour, day, week, month, year or a custom date range. Additional details can be shown by opening an expanded chart view. Historical data can be easily downloaded for viewing or consumption.

**Examples**

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160602104930/LineChartWidget.jpg" width="600" height="367" alt="Line Chart Tutorial"><br/></p>


#### Line Chart Arduino Tutorial

This tutorial explains how to use the Line Chart display widget to add a sensor connected to your Arduino.

Let’s look at each dropdown field that will be used when adding your sensor.

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160607143519/widget-tutorial-linechart-form-2.png" width="346" height="430" alt="Slider Tutorial Form"><br/><br/></p>

**Name** <br/>
Give your sensor a name. 

**Device** <br/>
Select your Arduino device.

**Connectivity** <br/>
Select your method of connectivity; is your sensor connected to Analog pins, or will it make use of the Cayenne Virtual pins? [Using Analog vs Virtual pins](http://www.cayenne-mydevices.com/CayenneStaging/docs/#using-analog-vs-virtual-pins)

   - **Analog** <br/>
If you’re trying to read data from an analog sensor, the Arduino may have several analog inputs that can be used. Simply connect your analog sensor to one of the analog pins on the Arduino. Make sure you select the correct corresponding pin when adding a widget for your analog sensor.
   - **Virtual** <br/>
[Virtual pins](http://www.cayenne-mydevices.com/CayenneStaging/docs/#virtual-pins-microcontrollers) are channels to send and receive different data types from and to the Arduino (e.g. SPI, I2C, 1-Wire and devices connected to Arduino expansion boards). There are 26 virtual pins available for each Arduino board.
**Data, Unit, Icon** <br/>
Select the Data type, the Units, and the Icon to be used for the widget. For example, a temperature sensor could have a Data type of temperature, Units of Celsius, and a thermometer Icon.

**Min Scale Value & Max Scale Value (optional)** <br/>
Input the minimum and maximum values that you’d like the line graph widget to use when displaying the range of data for your sensor. This can help improve the visualization of your sensor data as it displays on the line graph.

**Add Widget** <br/>
After filling in each of the fields for your widget, click **Add Widget** and the widget will be added to your dashboard.

**Sketch File** <br/>
[Arduino Line Chart Widget sketch file](https://github.com/myDevicesIoT/CayenneArduinoSamples/blob/master/CustomWidgets/LineChartWidget/LineChartWidget.ino)



### Value

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160601104311/widget-tutorial-valuedisplay-header.png" width="346" height="133" alt="Value Display Widget"><br/></p>

Displays a measurement value from a sensor or device. You can use settings to adjust the icon or unit information displayed in the widget.

**Example States**

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160602105133/Widget-ValueDisplay.jpg" width="600" height="260" alt="Value Display Widget"><br/></p>

#### Value Arduino Tutorial

This tutorial explains how to use the Value display widget to add a sensor connected to your Arduino.

Let’s look at each dropdown field that will be used when adding your sensor.

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160510063126/widget-tutorial-valuedisplay-form.png" width="346" height="500" alt="Value Display"><br/><br/></p>

**Name** <br/>
Give your sensor a name. 

**Device** <br/>
Select your Arduino device.

**Connectivity** <br/>
Select your method of connectivity; is your sensor connected to Analog pins, or will it make use of the Cayenne Virtual pins? [Using Analog vs Virtual pins](http://www.cayenne-mydevices.com/CayenneStaging/docs/#using-analog-vs-virtual-pins)

   - **Analog** <br/>
If you’re trying to read data from an analog sensor, the Arduino may have several analog inputs that can be used. Simply connect your analog sensor to one of the analog pins on the Arduino. Make sure you select the correct corresponding pin when adding a widget for your analog sensor.
   - **Virtual** <br/>
[Virtual pins](http://www.cayenne-mydevices.com/CayenneStaging/docs/#virtual-pins-microcontrollers) are channels to send and receive different data types from and to the Arduino (e.g. SPI, I2C, 1-Wire and devices connected to Arduino expansion boards). There are 26 virtual pins available for each Arduino board.
**Data, Unit, Icon** <br/>
Select the Data type, the Units, and the Icon to be used for the widget. For example, a temperature sensor could have a Data type of temperature, Units of Celsius, and a thermometer Icon.

**Add Widget** <br/>
After filling in each of the fields for your widget, click **Add Widget** and the widget will be added to your dashboard.

**Sketch File** <br/>
[Arduino Value Widget sketch file](https://github.com/myDevicesIoT/CayenneArduinoSamples/blob/master/CustomWidgets/ValueWidget/ValueWidget.ino)


### Gauge

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160601104412/widget-tutorial-gauge-header.png" width="346" height="124" alt="Gauge Widget"><br/></p>

Displays the current value of a sensor within a given range of values. Good, warning and danger value ranges can be defined in settings.

**Example States**

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160602105306/Widget-Gauge.jpg" width="600" height="367" alt="Gauge Widget"><br/></p>


#### Gauge Arduino Tutorial

This tutorial explains how to use the Gauge display widget to add a sensor connected to your Arduino.

Let’s look at each dropdown field that will be used when adding your sensor.

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160620105552/Widget-GaugeSettings.png" width="346" height="674" alt="Gauge Settings"><br/><br/></p>

**Name** <br/>
Give your sensor a name. 

**Device** <br/>
Select your Arduino device.

**I/O** <br/>
Select your method of connectivity; is your sensor connected to Analog pins, or will it make use of the Cayenne Virtual pins? [Using Analog vs Virtual pins](http://www.cayenne-mydevices.com/CayenneStaging/docs/#using-analog-vs-virtual-pins)

   - **Analog** <br/>
If you’re trying to read data from an analog sensor, the Arduino may have several analog inputs that can be used. Simply connect your analog sensor to one of the analog pins on the Arduino. Make sure you select the correct corresponding pin when adding a widget for your analog sensor.
   - **Virtual** <br/>
[Virtual pins](http://www.cayenne-mydevices.com/CayenneStaging/docs/#virtual-pins-microcontrollers) are channels to send and receive different data types from and to the Arduino (e.g. SPI, I2C, 1-Wire and devices connected to Arduino expansion boards). There are 26 virtual pins available for each Arduino board.
**Data, Unit, Icon** <br/>
Select the Data type, the Units, and the Icon to be used for the widget. For example, a temperature sensor could have a Data type of temperature, Units of Celsius, and a thermometer Icon.

**Minimum and Maximum Values (optional)**<br/>
Input the minimum and maximum values that you’d like the gauge widget to use when displaying the range of data for your sensor. This can help improve the visualization of your sensor data as it displays on the gauge widget.

**Step 1: Sketch File** <br/>
If you haven’t already uploaded the Gauge code for this widget to your Arduino, click the **Sketch File** button to open the [Gauge Widget sketch file](https://github.com/myDevicesIoT/CayenneArduinoSamples/blob/master/CustomWidgets/GaugeWidget/GaugeWidget.ino). See [Using Sketch Files](http://www.cayenne-mydevices.com/CayenneStaging/docs/#using-sketch-files-arduino) for more information on customizing and using sketch files.

**Step 2: Add Widget** <br/>
After filling in each of the fields for your widget, click **Add Widget** and the widget will be added to your dashboard.


### 2 State

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160601104431/widget-tutorial-2state-header.png" width="346" height="124" alt="2 State Widget"><br/></p>

Displays the current status of a device as either 1 (being High) or 0 (being low). An optional icon can be displayed in the widget.

**Example States**

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160602105446/2State.jpg" width="600" height="376" alt="2 State Widget"><br/></p>

#### 2 State Arduino Tutorial

This tutorial explains how to use the 2 State display widget to add a sensor connected to your Arduino.

Let’s look at each dropdown field that will be used when adding your sensor.

<p style="text-align:center"><br/><img src="http://d1nocd4j7qtmw4.cloudfront.net/wp-content/uploads/20160511050603/widget-tutorial-2state-form.png" width="346" height="490" alt="2 State Widget"><br/><br/></p>

**Name** <br/>
Give your sensor a name. 

**Device** <br/>
Select your Arduino device.

**Connectivity** <br/>
Select your method of connectivity; is your sensor connected to Digital pins, or will it make use of the Cayenne Virtual pins?

   - **Digital** <br/>
A digital pin can be used to read data from a non-analog sensor, but the data will need to be written to a virtual channel. If you’re trying to read data from a non-analog sensor, you’ll most likely use a virtual pin.
   - **Virtual** <br/>
[Virtual pins](http://www.cayenne-mydevices.com/CayenneStaging/docs/#virtual-pins-microcontrollers) are channels to send and receive different data types from and to the Arduino (e.g. SPI, I2C, 1-Wire and devices connected to Arduino expansion boards). There are 26 virtual pins available for each Arduino board.
**Data, Unit, Icon** <br/>
Select the Data type, the Units, and the Icon to be used for the widget. For example, a temperature sensor could have a Data type of temperature, Units of Celsius, and a thermometer Icon.

**Add Widget** <br/>
After filling in each of the fields for your widget, click **Add Widget** and the widget will be added to your dashboard.

**Sketch File** <br/>
[Arduino 2 State Widget sketch file](https://github.com/myDevicesIoT/CayenneArduinoSamples/blob/master/CustomWidgets/2StateWidget/2StateWidget.ino)


