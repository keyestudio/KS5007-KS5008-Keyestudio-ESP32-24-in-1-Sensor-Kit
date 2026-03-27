### Project 29: Intrusion Detection

![](media/b7828b9e5ee615a151567e20d35db90f.png)

**1. Description**

In this experiment, we use a PIR motion sensor to control an active buzzer to emit sounds and the onboard LED to flash rapidly.

**2. Required Components**

<table class="colwidths-auto docutils align-default">
<tbody>
<tr class="odd">
<td>


![](media/c9020c6015e55923afec197ab9d03fae.png)</td>
<td>

![](media/6d96c844b0260ad712130945d692a7a2.jpeg)</td>
<td>

![](media/256a8301b740dfb2981a635a4b575ba0.png)</td>
<td>

![](media/cbc890daba907eee365bdaacf1f509a8.png)</td>
</tr>
<tr class="even">
<td>ESP32 Board*1</td>
<td>ESP32 Expansion Board*1</td>
<td>Keyestudio DIY PIR Motion Sensor*1</td>
<td>Keyestudio DIY Active Buzzer*1</td>
</tr>
<tr class="odd">
<td>

![](media/12ecb079cf6481a6f0f04d6b7bb31fd8.png)</td>
<td>

![](media/0d81e07a0f67700c5a396fc7e1e614e1.jpeg)</td>
<td>

![](media/edbfec59fe015bd9987e4b4d542b466d.png)</td>
<td></td>
</tr>
<tr class="even">
<td>Keyestudio White LED Module*1</td>
<td>3P Dupont Wire*3</td>
<td>Micro USB Cable*1</td>
<td></td>
</tr>
</tbody>
</table>

**3. Connection Diagram**

![](media/07ded8ae2b9b12d7d399422cae6b8c5a.png)

**4. Test Code**


```Python
# Import Pin and time modules.
from machine import Pin 
import time 

# Define the pins of the Human infrared sensor,led and Active buzzer. 
sensor_pir = Pin(15, Pin.IN)
led = Pin(22, Pin.OUT)
buzzer = Pin(4, Pin.OUT)

while True: 
      if sensor_pir.value():
          print("Warning! Intrusion detected！")
          buzzer.value(1)
          led.value(1)
          time.sleep(0.2)
          buzzer.value(0)
          led.value(0)
          time.sleep(0.2)         
      else:
          buzzer.value(0)
          led.value(0)
```

**5. Test Result**

Connect the wires according to the experimental wiring diagram and power on. Click![](media/da852227207616ccd9aff28f19e02690.png)“Run current script”, the code starts executing. If the PIR Motion sensor detects someone moving nearby, the buzzer will emit an alarm , and the LED will flash continuously. At the same time, the “shell” will display“Warning\! Intrusion detected！”.

Press “Ctrl+C”or click ![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“Stop/Restart backend”to exit the program.

![](media/8d9889d04e7080f918446cc8a23d05e8.png)