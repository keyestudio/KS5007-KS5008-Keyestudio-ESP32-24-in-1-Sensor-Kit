### Project 6: Button Sensor

![](media\4d5f6ea741d1e346e03f6efe7cfc9d2d.jpeg)

**Overview**

In this kit, there is a Keyestudio single-channel button module, which mainly uses a tact switch and comes with a yellow button cap.

In previous lessons, we learned how to make the pins of our single-chip microcomputer output a high level or low level. In this experiment, we will read the high level (3.3V) and low level (0V).

We can determine whether the button on the sensor is pressed by reading the high and low level of the S terminal on the sensor.

**Working Principle**

![](media\a51debfc8a38d0d5729d1da394f95ca5.png)

The button module has four pins. The pin 1 is connected to the pin 3 and the pin 2 is linked with the pin 4. When the button is not pressed, they are disconnected. Yet, when the button is pressed, they are connected. If the button is released, the signal end
is high level.

**Components**

![image-20231020083206539](media\image-20231020083206539.png)


**Connection Diagram**

![](media\395caba95f49d582d7fd36cacbf44a7c.png)

**Test Code**


```c
//*************************************************************************************
/*
 * Filename    : button
 * Description : Read key value
 * Auther      : http://www.keyestudio.com
*/
int val = 0;  //Useto store key values
int button = 15; //The pin of the button is connected to GP15
void setup() {
  Serial.begin(9600); //Start the serial port monitor and set baud rate to 9600
  pinMode(button, INPUT); //Set key pin to input mode
}

void loop() {
  val = digitalRead(button);  //Read the value of the key and assign it to the variable val
  Serial.print(val);  //Print it on the serial port
  if (val == 0) { //Press the key to read the low level and print the press related information
    Serial.print("        ");
    Serial.println("Press the botton");
    delay(100);
  }

  else {  //Print information about key release
    Serial.print("        ");
    Serial.println("Loosen the botton");
    delay(100);
  }
}
//*************************************************************************************
```




**Code Explanation**

**1. pinMode(button, INPUT)**; set the pin of the button module to GP15 and INPUT.

Configure INPUT through pinMode(). INPUT must use the pull-up or pull-down resistor(ours module has the pull-up resistor R1).

**2. Serial.begin(9600)**: Initialize serial communication and set the baud rate to 9600.

**3. digitalRead(button)**: read the digital level of the button(HIGH or LOW). If this pin is not connected to pins, the digitalRead() will
return HIGH or LOW.

**4. if..else..**：if the logic behind () is true, execute the code of (); otherwise execute the code of **else**.

5\. If the button is pressed, the signal end is low level, GP15 is low level and Val is 0. Then the monitor will show the corresponding value and characters; otherwise, the sensor is released, val is 1 and monitor will show 1 and other characters

**Test Result**

Connect the wires according to the experimental wiring diagram, compile and upload the code to the ESP32. After uploading successfully，we will use a USB cable to power on，open the serial monitor and set the baud rate to 9600. The serial monitor will display the corresponding data and characters. When the button is pressed, val is 0, the monitor will show“Press the button”；when released, val is 1，the monitor will show“Loosen the button”; as shown below

![](media\bbd14736aa5700c252138d5b4c185568.png)