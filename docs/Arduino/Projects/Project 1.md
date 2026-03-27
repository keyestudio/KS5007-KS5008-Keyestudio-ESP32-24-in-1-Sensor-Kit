When we get the kit, we can see that there are 24 sensors/modules in the kit, which contain the corresponding ESP32 mainboard, ESP32 Expansion Board and wirings. Here, we will connect the 24 sensors individually to the ESP32 mainboard and the ESP32 Expansion Board using the wirings. Then run the corresponding code to test the function of each sensor separately. Our next projects are work to study the principles of individual modules/sensors from simple to complex as well as some extended applications of sensors to consolidate and deepen our understanding of the kits.

Note : When connecting the module/sensor wirings in the projects, the wiring method and position must be followed in the document. What’s more, do not misconnect the power supply and signal pins, otherwise there may be no experimental results or damage to the modules/sensors.  

### Project 1: Hello World

**Overview**

For ESP32 beginners, we will start with some simple things. In this project, you only need a ESP32 mainboard, a USB cable and a computer to complete the "Hello World\!" project, which is a test of communication between the ESP32 mainboard and the computer as well as a primary project.

**Components**

| ![image-20231113151026574](media/image-20231113151026574.png) | ![image-20231113151032312](media/image-20231113151032312.png) |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| ESP32*1                                                      | USB Cable*1                                                  |


**Wiring Diagram：**

In this project, we will use a USB cable to connect the ESP32 to a computer.

![image-20231020082805460](media\image-20231020082805460.png)

**Test Code**


```c
//*************************************************************************************
/*
 * Filename    : Hello World
 * Description : Enter the letter R,and the serial port displays"Hello World".
 * Auther      :http//www.keyestudio.com
*/
char val;// defines variable "val"
void setup()
{
Serial.begin(9600);// sets baudrate to 9600
}
void loop()
{
  if (Serial.available() > 0) {
    val=Serial.read();// reads symbols assigns to "val"
    if(val=='R')// checks input for the letter "R"
    {  // if so,    
     Serial.println("Hello World!");// shows “Hello World !”.
    }
  }
}
//*************************************************************************************
```

Before uploading the test code to the ESP32，click“Tools”→“Board”，select“ESP32 Wrover Module”.

![](media\fa56991b6368d175880603c446b81e2a.png)

Select the correct serial port.

![](media\1318a740375ee46c2bb9ec72bad3aeb7.png)

Note：For macOS users, if the upload fails, set the baud rate to 115200 before clicking ![](media\b0d41283bf5ae66d2d5ab45db15331ba.png).

![](media\97f4ac2f7d2aac69f5b5cd558668b307.png)

Click![](media\b0d41283bf5ae66d2d5ab45db15331ba.png)to upload the test code to the ESP32.

![](media\6e6ae41d4b07591efcb3c907958aa719.png)

Note: If the uploading code fails, you can press and hold the Boot button on the ESP32 after clicking![](media\d09c4a31563f04a42d451e7bc1a5fb8a.png)and release it after the percentage of uploading progress appears.![](media\dc77bfcf5851c8f43aab6cbe7cec7920.png), as shown below:  

![](media\157ee2e7687559d9812d24edec758150.png)

The code is uploaded successfully.

![](media\3511be64175bc28c8ab8a4a3b766e5c3.png)

**Test Result**

After uploading successfully，we will use a USB cable to power on，click![](media\2f6bca56f724e45a855335cb53ae9b4e.png) to enter the serial monitor and set the baud rate to 9600，enter the letter“R”，click“Send”，then the serial monitor prints“Hello World\!”.

![](media\cc9f1801ab1db618316fea36c8d9ed3b.png)