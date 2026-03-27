### Project 29: Intrusion Detection

![](media/b7828b9e5ee615a151567e20d35db90f.png)

**1. Description**

In this experiment, we use a PIR motion sensor to control an active buzzer to emit sounds and the onboard LED to flash rapidly.

**2. Required Components**

![image-20231020085335159](media/image-20231020085335159.png)

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