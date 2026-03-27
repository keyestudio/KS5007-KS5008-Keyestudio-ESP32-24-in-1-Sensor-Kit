### Project 38: Comprehensive Experiment

![](media/c92bfcbd1ecd7fe91198066d0c9a4df6.jpeg)

**1. Introduction**

We did a lot of experiments, and for each one we needed to re-upload the code, so can we achieve different functions through an experiment? In this experiment, we will use an external button module to achieve different function.

**2. Components Required**

<table class="colwidths-auto docutils align-default">
<tbody>
<tr class="odd">
<td>


![](media/c9020c6015e55923afec197ab9d03fae.png)</td>
<td>

![](media/6d96c844b0260ad712130945d692a7a2.jpeg)</td>
<td>

![](media/f0ef7a5a2e7eebb09e91f73cb2a6caf3.png)</td>
<td>

![](media/1aafa8910f5184973f1c913c19489fbd.png)</td>
<td>

![](media/a0eebfcd8f84c3fbac526e9910e66692.png)</td>
</tr>
<tr class="even">
<td>ESP32 Board*1</td>
<td>ESP32 Expansion Board*11</td>
<td>Keyestudio White LED Module*1</td>
<td>Keyestudio Button Module*1</td>
<td>Keyestudio Rotary Potentiometer*1</td>
</tr>
<tr class="odd">
<td>

![](media/b62846d9a80a7e7aed5ffbef0caedf7c.png)</td>
<td>

![](media/fb4fa5fdd5689ded9c213ba5ceb34c0d.png)</td>
<td>

![](media/4a358f0f161b2e4dcae43f9315902ef3.png)</td>
<td>

![](media/51729b3ba2184cf0ca0d3242199731ad.png)</td>
<td>

![](media/edbfec59fe015bd9987e4b4d542b466d.png)</td>
</tr>
<tr class="even">
<td>Keyestudio Obstacle Avoidance Sensor*1</td>
<td>Keyestudio DIY Joystick Module*1</td>
<td>Keyestudio HC-SR04 Ultrasonic sensor *1</td>
<td>Keyestudio DIY Common Cathode RGB Module *1</td>
<td>MicroUSB Cable*1</td>
</tr>
<tr class="odd">
<td>

![](media/0d81e07a0f67700c5a396fc7e1e614e1.jpeg)</td>
<td>

![](media/269c154eda332be03643bada56070124.jpeg)</td>
<td>

![](media/fc3fd9c0110b04d1af77a2ff8c01a10a.png)</td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>3P Dupont Wire*4</td>
<td>4P Dupont Wire*2</td>
<td>5P Dupont Wire*1</td>
<td></td>
<td></td>
</tr>
</tbody>
</table>

**3. Wiring Diagram**

![](media/b6956132b3e2e5bef697151f0de7656a.png)

**4. Test Code**


```Python
from machine import ADC, Pin, PWM
import time
import machine
import random

pwm_r = PWM(Pin(4))
pwm_g = PWM(Pin(0))
pwm_b = PWM(Pin(2))

pwm_r.freq(1000)
pwm_g.freq(1000)
pwm_b.freq(1000)

potentiometer_adc=ADC(Pin(33))
potentiometer_adc.atten(ADC.ATTN_11DB)
potentiometer_adc.width(ADC.WIDTH_12BIT)

button = Pin(23, Pin.IN)
led = PWM(Pin(5))
led.freq(1000)

Avoiding = Pin(14, Pin.IN, Pin.PULL_UP)

button_z=Pin(32,Pin.IN,Pin.PULL_UP)
rocker_x=ADC(Pin(35))
rocker_y=ADC(Pin(34))
rocker_x.atten(ADC.ATTN_11DB)
rocker_y.atten(ADC.ATTN_11DB)
rocker_x.width(ADC.WIDTH_12BIT)
rocker_y.width(ADC.WIDTH_12BIT)

# Set ultrasonic pins
trigger = Pin(13, Pin.OUT)
echo = Pin(12, Pin.IN)

def light(red, green, blue):
    pwm_r.duty(red)
    pwm_g.duty(green)
    pwm_b.duty(blue)

# Ultrasonic ranging, unit: cm
def getDistance(trigger, echo):
    # Generates a 10us square wave
    trigger.value(0)   #A short low level is given beforehand to ensure a clean high pulse:
    time.sleep_us(2)
    trigger.value(1)
    time.sleep_us(10)#After pulling high, wait 10 microseconds and immediately set it to low
    trigger.value(0)
    
    while echo.value() == 0: #Establish a while loop to detect whether the echo pin value is 0 and record the time at that time
        start = time.ticks_us()
    while echo.value() == 1: #Establish a while loop to check whether the echo pin value is 1 and record the time at that time
        end = time.ticks_us()
    d = (end - start) * 0.0343 / 2 #The travel time of the sound wave x the speed of sound (343.2 m/s, 0.0343 cm/microsecond), and the distance back and forth divided by 2
    return d


keys = 0
nums = 0
print(keys % 5)
def toggle_handle(pin):
    global keys
    keys += 1
    print(keys % 4)

button.irq(trigger = Pin.IRQ_FALLING, handler = toggle_handle)

def showRGB():
    R = random.randint(0,1023)
    G = random.randint(0,1023)
    B = random.randint(0,1023)
    light(R, G, B)
    time.sleep(0.3)

def showAvoiding():
    if Avoiding.value() == 0:
        print("0   There are obstacles")   #Press to print the corresponding information.
    else:
        print("1   All going well")
    time.sleep(0.1) #delay 0.1s
    
def showJoystick():
    B_value = button_z.value()
    X_value = rocker_x.read()
    Y_value = rocker_y.read()
    print("button:", end = " ")
    print(B_value, end = " ")
    print("X:", end = " ")
    print(X_value, end = " ")
    print("Y:", end = " ")
    print(Y_value)
    time.sleep(0.1)

def adjustLight():
    pot_value = potentiometer_adc.read()
    print(pot_value)
    led.duty(pot_value)
    time.sleep(0.1)

def showDistance():
    distance = getDistance(trigger, echo)
    print("The distance is ：{:.2f} cm".format(distance))
    time.sleep(0.1)

while True:
    nums = keys % 5  #number of keystrokes mod 5 to get 0, 1, 2, 3, 4 
    if nums == 0:  #According to RGB
        showRGB()
    elif nums == 1:  #Displays the high and low level of the Avoiding sensor
        showAvoiding()
    elif nums == 2: #Displays the rocker value
        showJoystick()
    elif nums == 3:  #The potentiometer adjusts the LED
        adjustLight()
    elif nums == 4:  #Display ultrasonic ranging value
        showDistance()      
```



**5. Code Explanation**

1\. Calculate how many times the button is pressed, divide it by 5, and get the remainder which is 0, 1 2, 3, and 4. According to different remainders, construct five unique functions to control the experiment and realize different functions.

2\. Following the instructions, we can add or remove sensors/modules in the wiring, and then change the experimental function in the code.

**6. Test Result**

Connect the wires according to the experimental wiring diagram and power on. Click ![](media/da852227207616ccd9aff28f19e02690.png)“Run current script”，the code starts executing. At the beginning, the number of the button is 0 and remainder is 0, RGB module will flash random color.

![](media/2b5ff126000d0182b9b3e6bd70de3bab.png)

Press the button, the RGB stops flashing, press once, the remainder is 1. The function of the project is whether the obstacle avoidance sensor detects obstacles and reads high and low levels. The monitor will display as follows:

![](media/5de8f3b186cd2cb256098d9b28799660.png)

Press the button again, the time of pressing buttons is 2 and the remainder is 2. Read digital values at x, y and z axis of the joystick module. As shown below;

![](media/21a31fba315990014bd6e62a4e1b78f6.png)

Press the key for the third time, the remainder is 3. Then the potentiometer can adjust the PWM value at the GPI05 port to control LED brightness of the purple LED.

![](media/320515f267fd42d37be2498ae7f15595.png)

Press the key for the fourth time, the remainder is 4. Then the ultrasonic sensor can detect distance, as shown below:

![](media/b7ebf58db51f94d52c4e843531beb348.png)

Press the key for the fifth time, the remainder is 0. Then the RGB will flash. If you press keys incessantly, remainders will change in a loop way. So does functions. Press “Ctrl+C”or click ![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“Stop/Restart backend”to exit the program.