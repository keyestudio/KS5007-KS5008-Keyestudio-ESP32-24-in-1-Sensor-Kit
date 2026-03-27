### Project 6: Button Sensor

![img](media/4d5f6ea741d1e346e03f6efe7cfc9d2d.jpeg?lastModify=1774484129)

**1. Overview**

In this kit, there is a Keyestudio single-channel button module, which mainly uses a tact switch and comes with a yellow button cap.

In previous lessons, we learned how to make the pins of our single-chip microcomputer output a high level or low level. In this experiment, we will read the high level (3.3V) and low level (0V).

We can determine whether the button on the sensor is pressed by reading the high and low level of the S terminal on the sensor.

**2. Working Principle**

The button module has four pins. The pin 1 is connected to the pin 3 and the pin 2 is linked with the pin 4. When the button is not pressed, they are disconnected. Yet, when the button is pressed, they are connected. If the button is released, the signal end is high level.

![img](media/a51debfc8a38d0d5729d1da394f95ca5.png?lastModify=1774484129)

**3. Components**





![img](media/c9020c6015e55923afec197ab9d03fae.png?lastModify=1774484129)</td> <td>

![img](media/6d96c844b0260ad712130945d692a7a2.jpeg?lastModify=1774484129)</td> <td>

![img](media/efcc7b40d80043b7b1f90ceaa8d73639.png?lastModify=1774484129)</td> <td>

![img](media/0d81e07a0f67700c5a396fc7e1e614e1.jpeg?lastModify=1774484129)</td> <td>

</td> </tr> <tr class="even"> <td>ESP32 Board1</td> <td>ESP32 Expansion Board1</td> <td>Keyestudio DIY Button Module1</td> <td>3P Dupont Wire1</td> <td>Micro USB Cable*1</td> </tr> </tbody> </table>

**4. Connection Diagram**

![img](media/395caba95f49d582d7fd36cacbf44a7c.png?lastModify=1774484129)

**5. Test Code**

```
from machine import Pin
import time

button = Pin(15, Pin.IN, Pin.PULL_UP)

while True:
    if button.value() == 0:
        print("You pressed the button!")   #Press to print the corresponding information.
    else:
        print("You loosen the button!")
    time.sleep(0.1) #delay 0.1s
```

**6. Code Explanation**

**button = Pin(15, Pin.IN, Pin.PULL_UP),** we define the pin of the button as GP15 and set to PULL-UP mode

We can use **button = Pin(15, Pin.IN) to set INPUT mode,** at this time, the pins are in high resistance state.

1. **button.value(),** read levels of buttons. Function returns High or Low
2. **if..else.. sentence,** when the logic judge is TRUE, the code under the if will be activated; otherwise, the code udder the else will be activated.
3. When ESP32 detects the button pressed, the signal end is low level(GP 15 is low level). **button.value() is 0.** If the ESP32 detects the button unpressed, **button.value()** is 1 and else sentence will be activated.

**7. Test Result**

Connect the wires according to the experimental wiring diagram and power on. Click ![img](media/da852227207616ccd9aff28f19e02690.png?lastModify=1774484129)“Run current script”, the code starts executing, the string will be displayed on the ”Shell“ window. When the button is pressed, the ”Shell“ window will show“You pressed the button!”；when the button is released，the ”Shell“ window will show“Loosen the button”; as shown below. Press “Ctrl+C”or click![img](media/27451c8a9c13e29d02bc0f5831cfaf1f.png?lastModify=1774484129)“Stop/Restart backend”to exit the program.

![img](media/ba199239c85c395f36e42612246288eb.png?lastModify=1774484129)