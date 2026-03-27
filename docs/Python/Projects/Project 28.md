### Project 28: Alarm Experiment

![](media/6db3cb7d3a91e700a3b651c1f0edb7a5.jpeg)

**1. Overview**

In the previous experiment, we control an output module though an input module. In this lesson, we will make an experiment that the active buzzer will emit sounds once an obstacle appears.

**2. Components**

<table class="colwidths-auto docutils align-default">
<tbody>
<tr class="odd">
<td>


![](media/c9020c6015e55923afec197ab9d03fae.png)</td>
<td>

![](media/6d96c844b0260ad712130945d692a7a2.jpeg)</td>
<td>

![](media/ac83d2c470cd6c345f17feed3bce5358.png)</td>
<td>

![](media/cbc890daba907eee365bdaacf1f509a8.png)</td>
<td>

![](media/0d81e07a0f67700c5a396fc7e1e614e1.jpeg)</td>
<td>

![](media/edbfec59fe015bd9987e4b4d542b466d.png)</td>
</tr>
<tr class="even">
<td>ESP32 Board*1</td>
<td>ESP32 Expansion Board*1</td>
<td>Keyestudio Obstacle Avoidance Sensor*1</td>
<td>Keyestudio Active Buzzer*1</td>
<td>3P Dupont Wire*2</td>
<td>Micro USB Cable*1</td>
</tr>
</tbody>
</table>

**3. Connection Diagram**

![](media/e37efdec9676d47eaf8dabd2da41759a.png)

**4. Test Code**

```Python
from machine import Pin
import time

buzzer = Pin(4, Pin.OUT)
sensor = Pin(15, Pin.IN)
while True:
    buzzer.value(not(sensor.value()))
    time.sleep(0.01)
```


**5. Code Explanation**

When an obstacle is detected, sensor.value() will return a low level signal. So when an obstacle is detected, the GPIO4 connected to the buzzer pin will output a high level signal, the buzzer will emit sounds.

**6. Test Result**

Connect the wires according to the experimental wiring diagram and power on. Click ![](media/da852227207616ccd9aff28f19e02690.png)“Run current script”, the code starts executing. The active buzzer will emit sound if detecting obstacles; otherwise, it won’t emit sound. Press “Ctrl+C”or click ![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“Stop/Restart backend”to exit the program.