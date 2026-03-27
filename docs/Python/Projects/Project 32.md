### Project 32: Sound Activated Light

![](media/f3ddb58e83a92a888d3e1d66f7456170.png)

**1. Introduction**

In this lesson, we will make a smart sound activated light using a sound sensor and an LED module. When we make a sound, the light will automatically turn on; when there is no sound, the lights will automatically turn off. How it works? Because the sound-controlled light is equipped with a sound sensor, and this sensor converts the intensity of external sound into a corresponding value. Then set a threshold, when the threshold is exceeded, the light will turn on, and when it is not exceeded, the light will go out.

**2. Components**

<table class="colwidths-auto docutils align-default">
<tbody>
<tr class="odd">
<td>


![](media/c9020c6015e55923afec197ab9d03fae.png)</td>
<td>

![](media/6d96c844b0260ad712130945d692a7a2.jpeg)</td>
<td>

![](media/cf7b54ba090f4e34025101cf9ece26d1.png)</td>
<td>

![](media/f0ef7a5a2e7eebb09e91f73cb2a6caf3.png)</td>
<td>

![](media/0d81e07a0f67700c5a396fc7e1e614e1.jpeg)</td>
<td>

![](media/edbfec59fe015bd9987e4b4d542b466d.png)</td>
</tr>
<tr class="even">
<td>ESP32 Board*1</td>
<td>ESP32 Expansion Board*1</td>
<td>Keyestudio Sound Sensor*1</td>
<td>Keyestudio White LED Module*1</td>
<td>3P Dupont Wire*2</td>
<td><p>MicroUSB</p>

<p>Cable*1</p></td>

</tr>
</tbody>
</table>

**3. Connection Diagram**

![](media/e54db9c861847ce0145accb574467c95.png)

**4. Test Code**

```Python
from machine import ADC, Pin
import time
 
# Turn on and configure the ADC with the range of 0-3.3V 
adc=ADC(Pin(34))
adc.atten(ADC.ATTN_11DB)
adc.width(ADC.WIDTH_12BIT)

led = Pin(15,Pin.OUT)

while True:
    adcVal=adc.read()
    print(adcVal)
    if adcVal > 600:
        led.value(1)
        time.sleep(3)
    else:
        led.value(0)
    time.sleep(0.1)
```


**5. Code Explanation**

We set the ADC threshold value to 600. If more than 600, LED will be on 3s; on the contrary, it will be off.

**6. Test Result**

Connect the wires according to the experimental wiring diagram and power on. Click ![](media/da852227207616ccd9aff28f19e02690.png)“Run current script”, the code starts executing. The shell monitor displays the corresponding volume ADC value. When the analog value of sound is greater than 600, the LED on the LED module will light up 3s, otherwise it will go off. Press “Ctrl+C”or click ![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“Stop/Restart backend”to exit the program.

![](media/ea65cb86fc3c75e71eabfb1f2e16fb1e.png)