### Project 18: Joystick Module

![](media\a28a09d0d9103cc8b93f2ae71f98482a.jpeg)

**Overview**

Game handle controllers are ubiquitous. There is a joystick module in this kit, which mainly uses PS2 joystick. When controlling it, we need to connect the X and Y ports of the module to the analog port of the single-chip microcomputer, port B to the digital port of the single-chip microcomputer, VCC to the power output port(3.3-5V), and GND to the GND of the MCU. We can read the high and low levels of two analog values and one digital port) to determine the working status of the joystick on the module.

In the project, two analog values(x axis and y axis) will be shown on Shell.

**Working Principle**

![](media\efcb8ed421ab3572af890d73788a8c01.jpeg)

In fact, its working principle is very simple. Its inside structure is equivalent to two adjustable potentiometers and a button. When this button is not pressed and the module is pulled down by R1, low levels will be output ; on the contrary, when the button is pressed, VCC will be connected (high levels). When we move the joystick, the internal potentiometer will adjust to output different voltages, and we can read the analog value.

**Components**

![image-20231020083906918](media\image-20231020083906918.png)


**Connection Diagram**

![](media\c1838e7013bc930e997d7684229bcea3.png)

**Test Code**


```c
//**********************************************************************************
/*  
 * Filename    : Joystick
 * Description : Read data from Rocker.
 * Auther      : http//www.keyestudio.com
*/
int xyzPins[] = {34, 35, 13};   //x,y,z pins
void setup() {
  Serial.begin(9600);
  pinMode(xyzPins[0], INPUT); //x axis. 
  pinMode(xyzPins[1], INPUT); //y axis. 
  pinMode(xyzPins[2], INPUT_PULLUP);   //z axis is a button.
}

// In loop(), use analogRead () to read the value of axes X and Y 
//and use digitalRead () to read the value of axis Z, then display them.
void loop() {
  int xVal = analogRead(xyzPins[0]);
  int yVal = analogRead(xyzPins[1]);
  int zVal = digitalRead(xyzPins[2]);
  Serial.println("X,Y,Z: " + String(xVal) + ", " +  String(yVal) + ", " + String(zVal));
  delay(500);
}
//**********************************************************************************
```




**Code Explanation**

In the experiment, according to the wiring diagram, the x pin is set to GPIO34, the y pin is set to GPIO35 and the pin of the joystick is set to GPIO13.

**Test Result**

Connect the wires according to the experimental wiring diagram, compile and upload the code to the ESP32. After uploading successfully，we will use a USB cable to power on. Open the serial monitor and set baud rate to 9600;

The serial monitor will show the corresponding value. Moving the joystick or pressing it will change the analog and digital values in the serial monitor.

![](media\06a9de681779df5cfc7e6bc24a928a3a.jpeg)

![](media\eefc7789bf77ba7056083fdca74abd10.png)