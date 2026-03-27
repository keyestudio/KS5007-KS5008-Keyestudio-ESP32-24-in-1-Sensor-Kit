### Project 30: Rotary Encoder control RGB

![](media/c6b4f1cedef06ed68d1c2e5ccf5c17d2.jpeg)

**1. Introduction**

In this lesson, we will control the LED on the RGB module to show different colors through a rotary encoder.

When designing the code, we need to divide the obtained values by 3 to get the remainders. The remainder is 0 and the LED will become red. The remainder is 1, the LED will become green. The remainder is 2, the LED will turn blue.

**2. Components**

<table class="colwidths-auto docutils align-default">
<tbody>
<tr class="odd">
<td>


![](media/c9020c6015e55923afec197ab9d03fae.png)</td>
<td>

![](media/6d96c844b0260ad712130945d692a7a2.jpeg)</td>
<td>

![](media/eb9d1b363af72bc105ce38cb9e4d99b1.png)</td>
<td>

![](media/989ee8ccd2a016dcaeb0bef68d55e912.png)</td>
</tr>
<tr class="even">
<td>ESP32Board*1</td>
<td>ESP32 Expansion Board*1</td>
<td><p>Keyestudio</p>

<p>Common Cathode RGB Module*1</p></td>

<td><p>Keyestudio</p>

<p>Rotary Encoder Module*1</p></td>

</tr>
<tr class="odd">
<td>

![](media/fc3fd9c0110b04d1af77a2ff8c01a10a.png)</td>
<td>

![](media/269c154eda332be03643bada56070124.jpeg)</td>
<td>

![](media/edbfec59fe015bd9987e4b4d542b466d.png)</td>
<td></td>
</tr>
<tr class="even">
<td>5P Dupont Wire*1</td>
<td>4P Dupont Wire*1</td>
<td>Micro USB Cable*1</td>
<td></td>
</tr>
</tbody>
</table>

**3. Connection Diagram**

![](media/c88ef3fa9019777e0697e242d0b41c4c.png)


**4. Add Library**

Open“Thonny”, click“This computer”→“D:”→“2.ESP32\_code\_MicroPython”→“lesson 44. Encoder control RGB”.
Select“<span style="color: rgb(255, 76, 65);">rotary\.py</span>”and“<span style="color: rgb(255, 76, 65);">rotary\_irq\_rp2.py</span>”，right-click and select“<span style="color: rgb(255, 76, 65);">**Upload to /**</span>”，waiting for the “<span style="color: rgb(255, 76, 65);">rotary\.py</span>”and“<span style="color: rgb(255, 76, 65);">rotary\_irq\_rp2.py</span>”to be uploaded to the ESP32.

![Img](media/img-20231010134724.png)
![Img](media/img-20231010134730.png)


**5. Test Code**


```Python
import time
from rotary_irq_rp2 import RotaryIRQ
from machine import Pin, PWM

pwm_r = PWM(Pin(0)) 
pwm_g = PWM(Pin(2))
pwm_b = PWM(Pin(15))

pwm_r.freq(1000)
pwm_g.freq(1000)
pwm_b.freq(1000)

def light(red, green, blue):
    pwm_r.duty(red)
    pwm_g.duty(green)
    pwm_b.duty(blue)

SW=Pin(27,Pin.IN,Pin.PULL_UP)
r = RotaryIRQ(pin_num_clk=12,
              pin_num_dt=14,
              min_val=0,
              reverse=False,
              range_mode=RotaryIRQ.RANGE_UNBOUNDED)

while True:
    val = r.value()
    print(val%3)
    if val%3 == 0:
        light(4950, 0, 0)
    elif val%3 == 1:
        light(0, 4950, 0)
    elif val%3 == 2:
        light(0, 0, 4950)
    time.sleep(0.1)
```


**6. Code Explanation**

In the experiment, we set the val to the remainder of Encoder\_Count divided by 3. Encoder\_Count is the value of the encoder. Then we can set pin GPIO0 (red), GPIO2 (green) and GPIO15 (blue) according to remainders.

Colors of the LEDs can be controlled by remainders.

**7. Test Result**

Connect the wires according to the experimental wiring diagram and power on. Click ![](media/da852227207616ccd9aff28f19e02690.png)“Run current script”, the code starts executing. Rotate the knob of the rotary encoder to display the reminders, which can control colors of LED(red green blue). Press
“Ctrl+C”or click ![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“Stop/Restart backend”to exit the program.

![](media/6894e2afd1eb7e150457048e0174adf8.png)