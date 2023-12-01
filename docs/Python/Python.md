# Python tutorial

## 1. Install Thonny：

Thonny is a free and open source software platform with small size, simple interface, simple operation and rich functions. It is a Python IDE suitable for beginners. In this tutorial, we use this IDE to develop a ESP32. Thonny supports multiple operating systems including Windows, Mac OS, Linux.

### 1. Download Thonny：

(1)  Enter the website：[https://thonny.org](https://thonny.org) to download the latest version of Thonny.
(2)  Thonny open-source code library：[https://github.com/thonny/thonny](https://github.com/thonny/thonny).

<table class="colwidths-auto docutils align-default">
<tbody>
<tr class="odd">
<td>System</td>
<td>Download link</td>
</tr>
<tr class="even">
<td>MAC OS：</td>
<td><a href="https://github.com/thonny/thonny/releases/download/v3.2.7/thonny-3.2.7.pkg">https://github.com/thonny/thonny/releases/download/v3.2.7/thonny-3.2.7.pkg</a></td>
</tr>
<tr class="odd">
<td>Windows：</td>
<td><a href=" https:/github.com/thonny/thonny/releases/download/v3.2.7/thonny-3.2.7.exe">https://github.com/thonny/thonny/releases/download/v3.2.7/thonny-3.2.7.exe</a></td>
</tr>
<tr class="even">
<td>Linux：</td>
<td><p>Latest version:</p>
<p><strong>Binary bundle for PC (Thonny+Python):</strong></p>
<p>bash &lt;(wget -O - https://thonny.org/installer-for-linux )</p>
<p><strong>With pip:</strong></p>
<p>pip3 install thonny </p>
<p><strong>Distro packages (may not be the latest version):</strong></p>
<p><strong>Debian, Rasbian, Ubuntu, Mint and others:</strong></p>
<p>sudo apt install thonny</p>
<p><strong>Fedora:</strong></p>
<p>sudo dnf install thonny</p></td>
</tr>
</tbody>
</table>

![](media/bd5823ede2c01d1fa4696438c62aec51.png)

### 2 Windows System

(1) The downloaded Thonny icon is as follows:
        
![](media/d3caa98d406fa06a124d5c98195b90db.png)

(2) Double-click“**thonny-3.3.13.exe**”and select install mode. You can choose ![](media/37be3f3bcc9aa0eb48c8b844eb46a71c.png).
    
![](media/4c044b255da8b14fe674eb9cce01627d.png)
    
(3) You can also keep selecting "**Next**" to finish install.
    
![](media/995b36640124b6a9b23f10473ff8a38a.png)
    
![](media/8bcc17840b9fc15d76f79fee8a0168ee.png)

(4) If you want to change the route of installing Thonny，just clic “**Browse...**”to select a new route and click "**OK**".
    
![](media/df6f63b42ebb1676b22c26b25dc9c7aa.png)
    
![](media/f5cd6d619b4645601c5b098ffdbec12a.png)
    
(5) Click "**Create desktop icon**" , you will view Thonny on your desktop.

![](media/a30c89dde3de81ad00aced30510071be.png)

(6) Click“**Install**”.
    
![](media/6ace65142291e5e8af5f81e4a6b2f180.png)

(7) Wait for a while but don’t click "**Cancel**".
    
![](media/a504b3a3ab16b4d91040cd5878acea0c.png)
    
(8) Click“**Finish**”.
    
![](media/a1fb6027e54a975de1c0aa1e1a0d6a29.png)
    
![](media/80f35044d91d66f734e36059db35f273.png)

### 3 Basic Setting：

Double-click Thonny, choose lanuage and initial settings and click "**Let’s go！**".
    
![](media/ee240978a4f844184f1ea9f5a21d0395.png)
    
![](media/619a856895d95e00beed748b1438072d.png)
    
![](media/bcf6c31e4f69c904a7a0c0e9df7e8d7d.png)

Click“**View**”→“**File**”and“**Shell**”.

![](media/5ff5c305585dbe7e832cc41183db5818.png)

![](media/d41b79772c9846fd8bf295c8451f8321.png)

![](media/3d04fe6893ca104e4e593a0786cb3799.png)

### 4 Install the CP2102 driver：

Before using the Thonny, we need to install the CP2102 driver in the computer.

**Windows system**

Check if the CP2102 driver has been installed

(1) Interface the ESP32 with your PC with a USB cable.

![](media/image-20230602171720765.png)

(2) Click“**This PC**”and right-click “**Manage**”.

![](media/84bc1f7d3169cad24b23d2ac620bc111.png)

(3) Click“**Device Manager**”, if the CP2102 driver has been installed，Silicon Labs CP210x USB to UART Bridge(COMx) will be shown.
    
![](media/a320816d8aed54304018d8380b5b6b3d.png)
    
If the CP2102 has not been installed.
    
![](media/776adb879fe6e299e3610cc92cfaf70b.png)
    
Click“**CP2102USB to UART Bridge Controller**”and “**Update driver**”.
    
![](media/7b342fbd38b03cba4dfce2045f4fe17b.png)
    
Click“**Browse my computer for drivers**”.
    
![](media/1cb9eaea189e4766d17a0a5977c23a74.png)
    
Click "**Browse...**" to choose Python Tutorials<span style="color: rgb(255, 76, 65);">\\1. Get started with Python\\CP2102 Driver File-Windows</span> and click "**Next**".
    
![](media/b1995fce2ccc024f32a9b9b83cbc28a6.png)
    
The CP2102 driver will be installed.
    
![](media/b99fbcb61c133392d1b94b65f51fc2c7.png)
    
![](media/da0dffd89b5f385612c3230422ee732f.png)

**MAC System**

You can refer to the file Get started with Arduino C，the route is：<span style="color: rgb(255, 76, 65);">KS5007(KS5008) Keyestudio ESP32 24 in 1&nbsp;Sensor Kit\\Windows\\Arduino\_C\\Get started with Arduino C before class C</span>.

![](media/33ad4ae8017abb0a971773df800077b5.png)

### 5 Burn Micropython firmware

To run a Python program on the ESP32 board, we need to burn the firmware to the ESP32 board first.

Download Micropython firmware microPython website：[http://micropython.org/](http://micropython.org/)

ESP32 firmware：[https://micropython.org/download/esp32/](https://micropython.org/download/esp32/)

![](media/c706d3cd6862323dcfccfd11ec7d1da3.png)

The firmware we use：**esp32-20210902-v1.17.bin**

Download firmware：[https://micropython.org/resources/firmware/esp32-20210902-v1.17.bin](https://micropython.org/resources/firmware/esp32-20210902-v1.17.bin)

Firmware：“<span style="color: rgb(255, 76, 65);">KS5007(KS5008)Keyestudio&nbsp;ESP32&nbsp;24 in1&nbsp;Sensor Kit\\Windows\\MicroPython\\1. Preparation before class for Python(Windows)\\Python\_Firmware</span>”.

![](media/d8fe3e12b4c55cfe927931182ae09109.png)

![](media/5ab965f5eff1672c8533d22537d6a52b.png)

**Burn the Micropython firmware**

Connect the ESP32 to your PC with a USB cable.

![](media/image-20230602171720765.png)

Make sure the driver has been installed successfully and the COM port can be identified correctly. Open "**Device Manager**" and  expand “**Ports**”.

![](media/d154c68ab7e252cf013b374069a2c6c0.png)

Open Thonny，click“**run**”and“**Select interpreter...**”

![](media/bda2bfc9d4576aef0b63e1f6373bf5a7.png)

Select "**Micropython (ESP32)**" and "**Silicon Labs CP210x USB to UART Bridge(COM3)**" and click “**Install or update firmware**”.

![](media/adfa634e977c803db209b18418f1df76.png)

Select“**Silicon Labs CP210x USB to UART Bridge(COM3)**”，click “**Browse...**”and choose the firmware "**esp32-20210902-v1.17.bin.**". Check“**Erase flash before installing**”and“**Flash mode**”，then click“**Install**”.

（<span style="color: rgb(255, 76, 65);">Note：</span> if you fail to install the firmware，press the Boot button on the ESP32 board and click“**Install**”.）

![](media/8b746aeb78c731ab638141c8c197437b.png)

![](media/d7f96e9e23e715bc64698227a88a1c1d.png)

![](media/055d392fe9a633564b3608128c7fd0a7.png)

Then click "**Close**" and "**OK**".

<span style="color: rgb(255, 76, 65);">Note：</span>During installation, you can press and hold the Boot button on the ESP32 mainboard. When the upload progress percentage appears, release the button for a while to complete the installation.

![](media/dc77bfcf5851c8f43aab6cbe7cec7920.png)

![](media/d6affc2fba3955d794ddbd19e0b57427.png)

![](media/5ff623e84c9a432edeb9534fe563f172.png)

![](media/7fc6ac0c25d55775ef60449f497c6f2f.png)

Turn off all windows and turn to the main page and click ![](media/a807dd85c760f2bda89025b9fd70156e.png)"**STOP**".

![](media/e9d1c2d43c22cf13ada2bdf4808aacb9.png)

**Test Code**

<span style="color: rgb(255, 169, 0);">Test the Shell commander</span>

Input <span style="color: rgb(255, 76, 65);">print('hello world')</span> in the“Shell”and press "**Enter**".

![](media/0dd4176ed13f85a7c96c14b4e20e6166.png)

<span style="color: rgb(255, 169, 0);">**Run the test code(online)**</span>

Connect the ESP32 to your PC. Users can program and debug programs withThonny.

Open Thonny and click "**Open**".

![](media/7fded176b193d1ac598571f7d16599f7.png)

When a new window pops up, click“**This computer**”.

![](media/101bf94e8e29ce5bc4a948f15b5dbe51.png)

Select the file“**lesson\_01\_HelloWorld.py**”.

![](media/26df9018f08a5fe68d82fd3b465a2759.png)

Click ![](media/31511be865975be04b53f27aa45c60a7.png), “Hello World”will be printed in the“**Shell**”monitor.

![](media/95686a34ef893fbad426628f8eedbdc6.png)

<span style="color: rgb(255, 76, 65);">Note: Press the reset button to reboot.</span>
<br>
<span style="color: rgb(255, 169, 0);">**Run the test code(offline)**</span>

After rebooting the ESP32, run the "**boot\.py**" file under the root directory first then run your code file.

So, we need to add a guide program to run the code of users.

Move the file <span style="color: rgb(255, 76, 65);">KS5007(KS5008)Keyestudio&nbsp;ESP32&nbsp;24 in 1&nbsp;Sensor Kit\\Windows\\MicroPython\\2. ESP32\_code\_MicroPython</span> to the disk(D)，the route is“<span style="color: rgb(0, 209, 0);">D:/2. ESP32\_code\_MicroPython</span>”.

![](media/000a950d20ba8d5cb478cbeb33dd238c.png)

Click lesson 00. Boot file and double-click "<span style="color: rgb(255, 76, 65);">boot\.py</span>", then the code under MicroPython device can run offline.

![](media/c5b03d591a7f0aaa8c4b5a6fc062d4df.png)

If you want to run the code offline, you nee to upload "<span style="color: rgb(255, 76, 65);">boot\.py</span>" and program code to MicroPython device, then press the ESP32’s reset button. We will take the lesson 00 and lesson 01 as an example. Select "<span style="color: rgb(255, 76, 65);">boot\.py</span>" and right-click "<span style="color: rgb(255, 76, 65);">**Upload to /**</span>".

![](media/6e7d162504c82e5300671a876741a5be.png)

![](media/d82442f19f4b80521ae5ff0af8e00617.png)

![](media/bd91aaba82d6016da9cbcbd76cc725ab.png)

Similarly, upload the lesson 01.HelloWorld\.py file to the “**MicroPython device**”.

![](media/bc116143d1a71e80834f9b8e62b06de5.png)

Press the Reset button, you will view code running in the **Shell** monitor.

![](media/7fda01d77b65bf60b0ac81fd84bb57c8.png)

<span style="color: rgb(255, 169, 0);">Upload the code to the ESP32</span>

We take the "**boot\.py**" as an example. If we add a "**boot\.py**" in each code directory, reboot the ESP32, the "**boot\.py**" will run first.

![](media/5d2bf5a1d5ca56a71a0f6fcaa5c65df8.png)

Select “**boot\.py**”in the file lesson 02. LED, right-click to select“**Upload to /**<span style="color: rgb(255, 76, 65);"></span>”. Then the code will be uploaded to the root directory of the ESP32 and click "**OK**".

![](media/fe76ba1fa40961eb080d5131ed6d3d0d.png)

![](media/6904b1cee8813cf845e6a24d59676c0c.png)

<span style="color: rgb(255, 169, 0);">Download the code to your PC</span>

left-click "**boot\.py**" of MicroPython device, then right-click "**Download to…**".

![](media/c48b47551a2aee4281802d387d0ec23d.png)

<span style="color: rgb(255, 169, 0);">Delete files of the ESP32</span>

For example, click“**boot\.py**”in the MicroPython device and right-click "**Delete**".

![](media/45e9295accb579e9cb7af9d2ea945c5d.png)

Select "**boot\.py**" in the lesson 02. LED folder, right-click "**Move to Recycle Bin**" to delete it.

![](media/cfc038e50113a6e1a4c570bc825f33ee.png)

<span style="color: rgb(255, 169, 0);">Create and save code</span>

Click“**File**”→“**New**”to create and edit code.

![](media/1d71df4720f9455dcaf17a72ec38bb1b.png)

Enter the code in the new file. We take the lesson 02. LED\.py as an example.

![](media/633604e1e66add9e335c3f0632231e07.png)

Click ![](media/40348c4ef49beb5e90593df6050c1d62.png) to save the code to your PC or the ESP32.

![](media/f6e3726933740f4a667a25463d696ba9.png)

Select "**MicroPython device**" and enter "**main\.py**" in the new page and click "**OK**".

![](media/895a782664e10406ce2ab9ba18507d19.png)

Then the code will be uploaded to the ESP32.

![](media/fbb3819dca237caca2c8a2ecd3d5587f.png)

Disconnect the USB cable and connect it, you can see the effect of the LED flashing continuously in the circuit on a cycle.  
![Img](./media/img-20231010102236.png)



## 2. Single Sensor/Experiment Projects：

When we get the kit, we can see that there are 24 sensors/modules in the kit, which contain the corresponding ESP32 mainboard, ESP32 Expansion Board and wirings. Here, we will connect the 24 sensors individually to the ESP32 mainboard and the ESP32 Expansion Board using a wiring. Then run the corresponding test code to test the function of each sensor separately. Our next lesson is to study the principles of individual modules/sensors from simple to complex as well as some extended applications of sensors to consolidate and deepen our understanding of the kits.  

<span style="color: rgb(255, 76, 65);">Note :</span> When connecting the module/sensor wirings in the experiment, the wiring method and position must be followed in the document. What’s more, do not misconnect the power supply and signal pin, otherwise there may be no experimental results or damage to the modules/sensors.  

### Project 1: Hello World

**1. Overview**

For ESP32 beginners, we will start with some simple things. In this project, you only need a ESP32 mainboard, a USB cable and a computer to complete the "Hello World\!" project, which is a test of communication between the ESP32 mainboard and the computer as well as a primary project.

**2. Components**

<table class="colwidths-auto docutils align-default">
<tbody>
<tr class="odd">
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/56053f7126905c6def63919c661d5c0a.jpeg"  /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/3bdcc62cfa661d2b860a76e28537e21e.png" style="width:1.41667in;height:0.76042in" /></td>
</tr>
<tr class="even">
<td>ESP32*1</td>
<td>USB Cable*1</td>
</tr>
</tbody>
</table>

**3. Wiring Diagram**

In this project, we will use a USB cable to connect the ESP32 to a computer.

![](media/image-20230602171720765.png)

**4. Running code online**

To run the ESP32 online, you need to connect the ESP32 to the computer, which allows you to compile or debug programs using Thonny software.  

<span style="color: rgb(255, 169, 0);">Advantages:</span>

1\. You can use the Thonny software to compile or debug programs.

2\. Through the "Shell" window, you can view error messages and output results generated during the running of the program as well as query related function information online to help improve the program.  

<span style="color: rgb(255, 169, 0);">Disadvantages:</span>

1\. To run the ESP32 online, you must connect the ESP32 to a computer and run it with the Thonny software.  
    
2\. If the ESP32 is disconnected from the computer , when they reconnect, the program won't run again.  

<span style="color: rgb(255, 76, 65);">Basic Operation:</span>

1\. Open Thonny and click“Open...”.
    
![](media/319b34bcc43d038d633af9acba0c198c.png)

2\. Click“This computer”in the new pop-up window.
    
![](media/5bdbc66ef89b41a53e46696c07b2c282.png)

In the new dialog box，select“Project\_01\_HelloWorld.py”,click“Open”. The code used in this tutorial is saved in the file **KS5007(KS5008)Keyestudio ESP32 24 in 1 Sensor Kit\\Windows\\MicroPython\\2.ESP32\_code\_MicroPython**. You can move the code to anywhere, for example, we can save the**2.ESP32\_code\_MicroPython in the** Disk(D), the route is <span style="color: rgb(255, 76, 65);">**D:\\2.ESP32\_code\_MicroPython.**</span>（The code in this tutorial is saved in the Disk(D) on your computer）

![](media/f26168c6fbf3638ab82e8ab5fcb8abba.png)

![](media/42e7ab8155f0df7a56ac57ab5ed97d00.png)

3\. Click![](media/da852227207616ccd9aff28f19e02690.png)“Run current script”to execute the program“Hello World\!”, "Welcome Keyestudio" , which will be printed in the“Shell”window.
    
![](media/c87d49e498df065dd42dbf32c2eec7ad.png)

**5. Exit running online**

When running online, click![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png) “Stop /Restart Backend”or press “Ctrl+C”on the Thonny to exit the program.  

![](media/db5de333b3cd58609dcca10a9382155c.png)

**6. Test Code**

```Python
print("Hello World!")
print("Welcome Keyestudio")
```

### Project 2: Lighting up LED

![](media/ce8d61c97eb89c94c05cc1f6299316b5.jpeg)

**1. Overview**

In this kit, we have a Keyestudio Purple Module, which is very simple to control. If you want to light up the LED, you just need to make a certain voltage across it.

In the project, we will control the high and low level of the signal end S through programming, so as to control the LED on and off. 

**2. Working Principle**

The two circuit diagrams are given.

The left one is wrong wiring-up diagram. Why? Theoretically, when the S terminal outputs high levels, the LED will receive the voltage and light up.

Due to limitation of IO ports of ESP32 board, weak current can’t make LED brighten.

The right one is correct wiring-up diagram. GND and VCC are powered up. When the S terminal is a high level, the triode Q1 will be connected and LED will light up(note: current passes through LED and R3 to reach GND by VCC not IO ports). Conversely, when the S terminal is a low level, the triode Q1 will be disconnected and LED will go off.

![](media/d205e9ad7c33cc55909cb1d652d42ad7.png)

**3. Components**

<table class="colwidths-auto docutils align-default">
<tbody>
<tr class="odd">
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/c9020c6015e55923afec197ab9d03fae.png" style="width:1.20833in;height:0.55903in" alt="4" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/6d96c844b0260ad712130945d692a7a2.jpeg" style="width:1.40903in;height:1.07917in" alt="ks0465-1" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/12ecb079cf6481a6f0f04d6b7bb31fd8.png" style="width:1.2in;height:0.93889in" alt="白色LED模块" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/0d81e07a0f67700c5a396fc7e1e614e1.jpeg" style="width:0.88056in;height:0.32083in" alt="3p线" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/edbfec59fe015bd9987e4b4d542b466d.png" style="width:0.83611in;height:0.44792in" alt="USB线" /></td>
</tr>
<tr class="even">
<td>ESP32 Board*1</td>
<td>ESP32 Expansion Board*1</td>
<td>Keyestudio White LED Module*1</td>
<td>3P Dupont Wire*1</td>
<td><p>Micro</p>
<p>USB Cable*1</p></td>
</tr>
</tbody>
</table>

**4. Wiring Diagram**

![](media/fed849dd5952f3b94a591d5bc5e64267.png)

**5. Test Code**

```Python
from machine import Pin
import time

led = Pin(0, Pin.OUT)# Build an LED object, connect the external LED light to pin 0, and set pin 0 to output mode
while True:
    led.value(1)# turn on led
    time.sleep(1)# delay 1s
    led.value(0)# turn off led
    time.sleep(1)# delay 1s
```

**6. Code Explanation**

1. **Machine** module is indispensable, we use **import machine** or **from machine import...** to program ESP32 with microPython.

2.  **time.sleep()** function is used to set delayed time, as **time.sleep(0.01),** which means, the delayed time is 10ms.

3.  **led = Pin(0, Pin.OUT)**，created a pin example and we name **led** . **0** is indicative of connected pin GP0，**Pin.OUT represents output mode**， can use **.value() to output high levels** (3.3V)**led.value(1) or low levels** (0V)**led.value(0)**。

4. **while True** is loop function，It means that sentences under this function will loop unless **True** changes into **False.** For the function **while**，**led.value(1)**，outputs high levels to the pin 0; then LED lights up. Then the delayed function **time.sleep(1)** will wait for 1s. When **led.value(0)** output low levels to the pin 0, the LED will go off，and the function **time.sleep(1)** will wait for 1s, cyclically, and LED will flash.

**7. Test Result**

Connect the wires according to the experimental wiring diagram and power on. Click ![](media/da852227207616ccd9aff28f19e02690.png)“Run current script”, the code starts executing, we will see that the LED in the circuit will flash alternately. Press “Ctrl+C”or click![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“Stop/Restart backend”to exit the program.

### Project 3: Traffic Lights Module

![](media/e191c790f251715b418bcfd39a32917f.jpeg)

**1. Overview**

In this lesson, we will learn how to control multiple LED lights and simulate the operation of traffic lights.

Traffic lights are signal devices positioned at road intersections, pedestrian crossings, and other locations to control flows of traffic.

In this kit, we will use the traffic light module to simulate the traffic light.

**2. Working Principle**

In previous lesson, we already know how to control an LED. In this part, we only need to control three separated LEDs. Input high levels to the signal R(3.3V), then the red LED will be on.

![](media/1479f32d51a02c2230cb535197093d4c.png)

**3. Components**

<table class="colwidths-auto docutils align-default">
<tbody>
<tr class="odd">
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/c9020c6015e55923afec197ab9d03fae.png" style="width:1.20833in;height:0.55903in" alt="4" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/6d96c844b0260ad712130945d692a7a2.jpeg" style="width:1.40903in;height:1.07917in" alt="ks0465-1" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/6ff6e93b37472de2695aefed0939a14e.png" style="width:1.45833in;height:0.801736in" alt="交通灯模块" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/fc3fd9c0110b04d1af77a2ff8c01a10a.png" style="width:0.95208in;height:0.39861in" alt="5p线" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/edbfec59fe015bd9987e4b4d542b466d.png" style="width:0.85972in;height:0.36875in" alt="USB线" /></td>
</tr>
<tr class="even">
<td>ESP32 Board*1</td>
<td>ESP32 Expansion Board*1</td>
<td>Keyestudio DIY Traffic Lights Module*1</td>
<td>5P Dupont Wire*1</td>
<td>Micro USB Cable*1</td>
</tr>
</tbody>
</table>

**4. Wiring Diagram**
    
![](media/cecade99c652fe14ea7547b80849f5b7.png)

**5. Test Code**

```Python
import machine
import time

led_red = machine.Pin(15, machine.Pin.OUT)
led_yellow = machine.Pin(2, machine.Pin.OUT)
led_green = machine.Pin(0, machine.Pin.OUT)

while True:
    led_green.value(1) # green light turn on
    time.sleep(5) # delay 5s
    led_green.value(0) # green light turn off
    for i in range(3): # yellow light blinks 3 times
        led_yellow.value(1)
        time.sleep(0.5)
        led_yellow.value(0)
        time.sleep(0.5)
    led_red.value(1) # red light turn on
    time.sleep(5) # delay 5s
    led_red.value(0) #red light turn off
```

**6. Code Explanation**

Create pins, set pins mode and delayed functions.

We use the **for** loop.

The simplest form is **for i in range()**.

In the code, we used range(3), which means the variable i starts from 0, increase 1 for each time, to 2.

**7. Test Result**

Connect the wires according to the experimental wiring diagram and power on. Click ![](media/da852227207616ccd9aff28f19e02690.png)“Run current script”, the code starts executing, we will see that the green LED will be on for 5s then off, the yellow LED will flash for 3s then go off and the red one will be on for 5s then off. Press “Ctrl+C”or click![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“Stop/Restart backend”to exit the program.

### Project 4: Breathing LED

![](media/25107e92a36e701f271b2371359f2679.jpeg)

**1. Overview**

A“breathing LED”is a phenomenon where an LED's brightness smoothly changes from dark to bright and back to dark, continuing to do so and giving the illusion of an LED“breathing. This phenomenon is similar to a lung breathing in and out. So how to control LED’s brightness? We need to take advantage of PWM. You may refer to Project 5.

**2. Components**

<table class="colwidths-auto docutils align-default">
<tbody>
<tr class="odd">
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/c9020c6015e55923afec197ab9d03fae.png" style="width:1.05278in;height:0.48819in" alt="4" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/6d96c844b0260ad712130945d692a7a2.jpeg" style="width:1.34444in;height:1.02986in" alt="ks0465-1" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/f0ef7a5a2e7eebb09e91f73cb2a6caf3.png" style="width:1.04931in;height:0.76528in" alt="白色LED模块" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/0d81e07a0f67700c5a396fc7e1e614e1.jpeg" style="width:0.98958in;height:0.36042in" alt="3p线" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/edbfec59fe015bd9987e4b4d542b466d.png" style="width:1.18819in;height:0.63681in" alt="USB线" /></td>
</tr>
<tr class="even">
<td>ESP32 Board*1</td>
<td>ESP32 Expansion Board*1</td>
<td>Keyestudio White LED Module*1</td>
<td>3P Dupont Wire*1</td>
<td>MicroUSB Cable*1</td>
</tr>
</tbody>
</table>

**3. Connection Diagram**

![](media/fed849dd5952f3b94a591d5bc5e64267.png)

**4. Test Code**


```Python
import time
from machine import Pin,PWM

#The way that the ESP32 PWM pins output is different from traditionally controllers.
#It can change frequency and duty cycle by configuring PWM’s parameters at the initialization stage.
#Define GPIO 0’s output frequency as 10000Hz and its duty cycle as 0, and assign them to PWM.
pwm =PWM(Pin(0,Pin.OUT),10000)

try:
    while True:
#The range of duty cycle is 0-1023, so we use the first for loop to control PWM to change the duty
#cycle value,making PWM output 0% -100%; Use the second for loop to make PWM output 100%-0%.  
        for i in range(0,1023):
            pwm.duty(i)
            time.sleep_ms(1)
            
        for i in range(0,1023):
            pwm.duty(1023-i)
            time.sleep_ms(1)  
except:
#Each time PWM is used, the hardware Timer will be turned ON to cooperate it. Therefore, after each use of PWM,
#deinit() needs to be called to turned OFF the timer. Otherwise, the PWM may fail to work next time.
    pwm.deinit()
```


**5. Test Result**

Connect the wires according to the experimental wiring diagram and power on. Click ![](media/da852227207616ccd9aff28f19e02690.png)“Run current script”, the code starts executing, we will see that the LED on the module gradually gets dimmer then brighter, cyclically, like human breathe. Press “Ctrl+C”or click![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“Stop/Restart backend”to exit the program.

### Project 5: RGB Module

![](media/b3515a7e0340f391bef256c9ed6ccd4b.jpeg)

**1. Overview**

Among these modules is a RGB module. It adopts a F10-full color RGB foggy common cathode LED. We connect the RGB module to the PWM port of MCU and the other pin to GND(for common anode RGB, the rest pin will be connected to VCC). So what is PWM?

PWM is a means of controlling the analog output via digital means. Digital control is used to generate square waves with different duty cycles (a signal that constantly switches between high and low levels) to control the analog output. In general, the input voltages of ports are 0V and 5V. What if the 3V is required? Or a switch among 1V, 3V and 3.5V? We cannot change resistors constantly. For this reason, we resort to PWM.

![](media/bbcfcb9ae56abb7e80ee587246fc4be9.GIF)

For Arduino digital port voltage outputs, there are only LOW and HIGH levels, which correspond to the voltage outputs of 0V and 5V respectively. You can define LOW as“0”and HIGH as“1’, and let the Arduino output five hundred‘0’or“1”within 1 second. If output five hundred‘1’, that is 5V; if all of which is‘0’,that is 0V; if output 25001 pattern, that is 2.5V.

This process can be likened to showing a movie. The movie we watch are not completely continuous. Actually, it generates 25 pictures per second, which cannot be told by human eyes. Therefore, we mistake it as a continuous process. PWM works in the same way. To output different voltages, we need to control the ratio of 0 and 1. The more ‘0’or‘1’ output per unit time, the more accurate the control.

**2. Working Principle**

For our experiment, we will control the RGB module to display different colors through three PWM values.

![](media/71e990d503b6f1822379091a37f58a6b.jpeg)

**3. Components**

<table class="colwidths-auto docutils align-default">
<tbody>
<tr class="odd">
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/c9020c6015e55923afec197ab9d03fae.png" style="width:1.05278in;height:0.48819in" alt="4" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/6d96c844b0260ad712130945d692a7a2.jpeg" style="width:1.34444in;height:1.02986in" alt="ks0465-1" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/51729b3ba2184cf0ca0d3242199731ad.png" style="width:1.15972in;height:0.88125in" alt="共阴RGB模块" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/269c154eda332be03643bada56070124.jpeg" style="width:1.03264in;height:0.40278in" alt="4p线" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/edbfec59fe015bd9987e4b4d542b466d.png" style="width:0.8875in;height:0.47569in" alt="USB线" /></td>
</tr>
<tr class="even">
<td>ESP32 Board*1</td>
<td>ESP32 Expansion Board*1</td>
<td>Keyestudio Common Cathode RGB Module *1</td>
<td>4P Dupont Wire*1</td>
<td>Micro USB Cable*1</td>
</tr>
</tbody>
</table>

**4. Connection Diagram**
    
![](media/e684c10368af661546702f94e0a495f3.png) 

**5. Test Code**

```Python
# import Pin, PWM and Random function modules.
from machine import Pin, PWM
from random import randint
import time

#Configure ouput mode of GPIO0, GPIO2 and GPIO15 as PWM output and PWM frequency as 10000Hz.
pins = [0, 2, 15]

pwm0 = PWM(Pin(pins[0]),10000)  
pwm1 = PWM(Pin(pins[1]),10000)
pwm2 = PWM(Pin(pins[2]),10000)

#define a function to set the color of RGBLED.
def setColor(r, g, b):
    pwm0.duty(1023-r)
    pwm1.duty(1023-g)
    pwm2.duty(1023-b)
    
try:
    while True:
        red   = randint(0, 1023) 
        green = randint(0, 1023)
        blue  = randint(0, 1023)
        setColor(red, green, blue)
        time.sleep_ms(200)
except:
    pwm0.deinit()
    pwm1.deinit()
    pwm2.deinit()
```

**6. Test Result**

Connect the wires according to the experimental wiring diagram and power on. Click ![](media/da852227207616ccd9aff28f19e02690.png)“Run current script”, the code starts executing, we will see that the RGB LED on the module starts to display random colors. Press “Ctrl+C”or click![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“Stop/Restart backend” to exit the program.

### Project 6: Button Sensor

![](media/4d5f6ea741d1e346e03f6efe7cfc9d2d.jpeg)

**1. Overview**

In this kit, there is a Keyestudio single-channel button module, which mainly uses a tact switch and comes with a yellow button cap.

In previous lessons, we learned how to make the pins of our single-chip microcomputer output a high level or low level. In this experiment, we will read the high level (3.3V) and low level (0V).

We can determine whether the button on the sensor is pressed by reading the high and low level of the S terminal on the sensor.

**2. Working Principle**

The button module has four pins. The pin 1 is connected to the pin 3 and the pin 2 is linked with the pin 4. When the button is not pressed, they are disconnected. Yet, when the button is pressed, they are connected. If the button is released, the signal end is high level.

![](media/a51debfc8a38d0d5729d1da394f95ca5.png)

**3. Components**

<table class="colwidths-auto docutils align-default">
<tbody>
<tr class="odd">
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/c9020c6015e55923afec197ab9d03fae.png" style="width:1.05278in;height:0.48819in" alt="4" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/6d96c844b0260ad712130945d692a7a2.jpeg" style="width:1.34444in;height:1.02986in" alt="ks0465-1" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/efcc7b40d80043b7b1f90ceaa8d73639.png" style="width:1.13611in;height:0.84722in" alt="单路按键模块" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/0d81e07a0f67700c5a396fc7e1e614e1.jpeg" style="width:0.91736in;height:0.33333in" alt="3p线" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/edbfec59fe015bd9987e4b4d542b466d.png" style="width:0.99167in;height:0.53125in" alt="USB线" /></td>
</tr>
<tr class="even">
<td>ESP32 Board*1</td>
<td>ESP32 Expansion Board*1</td>
<td>Keyestudio DIY Button Module*1</td>
<td>3P Dupont Wire*1</td>
<td>Micro USB Cable*1</td>
</tr>
</tbody>
</table>

**4. Connection Diagram**

![](media/395caba95f49d582d7fd36cacbf44a7c.png)

**5. Test Code**


```Python
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

**button = Pin(15, Pin\.IN, Pin.PULL\_UP),** we define the pin of the button as GP15 and set to PULL-UP mode

We can use **button = Pin(15, Pin\.IN) to set INPUT mode,** at this time, the pins are in high resistance state.

1.  **button.value(),** read levels of buttons. Function returns High or Low
    
2.  **if..else.. sentence,** when the logic judge is TRUE, the code under the if will be activated; otherwise, the code udder the else will be activated.
    
3.  When ESP32 detects the button pressed, the signal end is low level(GP 15 is low level). **button.value() is 0.** If the ESP32 detects the button unpressed, **button.value()** is 1 and else sentence will be activated.

**7. Test Result**

Connect the wires according to the experimental wiring diagram and power on. Click ![](media/da852227207616ccd9aff28f19e02690.png)“Run current script”, the code starts executing, the string will be displayed on the ”Shell“ window. When the button is pressed, the ”Shell“ window will show“You pressed the button\!”；when the button is released，the ”Shell“ window will show“Loosen the button”; as shown below. Press “Ctrl+C”or click![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“Stop/Restart backend”to exit the program.

![](media/ba199239c85c395f36e42612246288eb.png)

### Project 7: Obstacle Avoidance Sensor

![](media/e6dda88bb6faf8fc06d81361b7f48a3d.jpeg)

**1. Overview**

In this kit, there is a Keyestudio obstacle avoidance sensor, which mainly uses an infrared emitting and a receiving tube. In the experiment, we will determine whether there is an obstacle by reading the high and low level of the S terminal on the sensor.

**2. Working Principle**

NE555 circuit provides IR signals with frequency to the emitter TX, then the IR signals will fade with the increase of transmission distance. If encountering the obstacle, it will be reflected back.

When the receiver RX meets the weak signals reflected back, the receiving pin will output high levels, which indicates the obstacle is far away. On the contrary, it the reflected signals are stronger, low levels will be output, which represents the obstacle is close. There are two potentiometers on the module, and by adjusting the two potentiometers, we can adjust its effective distance.

![](media/f32ebd19bd8e893ab6c865f83b274900.png)

**3. Components**

<table class="colwidths-auto docutils align-default">
<tbody>
<tr class="odd">
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/c9020c6015e55923afec197ab9d03fae.png" style="width:1.05278in;height:0.48819in" alt="4" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/6d96c844b0260ad712130945d692a7a2.jpeg" style="width:1.34444in;height:1.02986in" alt="ks0465-1" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/b62846d9a80a7e7aed5ffbef0caedf7c.png" style="width:1.24167in;height:0.82083in" alt="避障传感器" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/0d81e07a0f67700c5a396fc7e1e614e1.jpeg" style="width:0.98958in;height:0.36042in" alt="3p线" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/edbfec59fe015bd9987e4b4d542b466d.png" style="width:0.8875in;height:0.47569in" alt="USB线" /></td>
</tr>
<tr class="even">
<td>ESP32 Board*1</td>
<td>ESP32 Expansion Board*1</td>
<td>Keyestudio DIY Obstacle Avoidance Sensor*1</td>
<td>3P Dupont Wire*1</td>
<td>Micro USB Cable*1</td>
</tr>
</tbody>
</table>

**4. Connection Diagram**

![](media/1c80fc2e1d7c038f0e105164090b97da.png)

**5. Test Code**

```Python
from machine import Pin
import time

sensor = Pin(15, Pin.IN)
while True:
    if sensor.value() == 0:
        print("There are obstacles")
    else:
        print("All going well")
    time.sleep(0.1)
```



**6. Code Explanation**

<span style="color: rgb(255, 76, 65);">Note:</span>

Connect the wires according to the connection diagram. After powering on, we start to adjust the two potentiometers to sense distance.


**7. Test Result**

Connect the wires according to the experimental wiring diagram and power on. Click ![](media/da852227207616ccd9aff28f19e02690.png)“Run current script”, the code starts executing, the string will be displayed in the ”Shell“ window. When the sensor detects the obstacle, sensor.value() is 0，the shell will show“There are obstacles”, if the obstacle is not detected, sensor.value () is 1,“All going well”will be shown, as shown below.
Press “Ctrl+C”or click![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“Stop/Restart backend”to exit the program.

![](media/86fc39da5df74b72325d5daddff5af70.png)

### Project 8: Tilt Module

![](media/9d4fcf498d8943539935d0f9638f22eb.jpeg)

**1. Overview**

In this kit, there is a Keyestudio tilt sensor. The tilt switch can output signals of different levels according to whether the module is tilted. There is a ball inside. When the switch is higher than the horizontal level, the switch is turned on, and when it is lower than the horizontal level, the switch is turned off. This tilt module can be used for tilt detection, alarm or other detection.

**2. Working Principle**

The working principle is pretty simple. When pin 1 and 2 of the ball switch P1 are connected, the signal S is low level and the red LED will light up; when they are disconnected, the pin will be pulled up by the 4.7K R1 and make S a high level, then LED will be off.

![](media/7b5da31ecdd90419d5b3326eebdb14e7.png)

**3. Components**

<table class="colwidths-auto docutils align-default">
<tbody>
<tr class="odd">
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/c9020c6015e55923afec197ab9d03fae.png" style="width:1.05278in;height:0.48819in" alt="4" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/6d96c844b0260ad712130945d692a7a2.jpeg" style="width:1.34444in;height:1.02986in" alt="ks0465-1" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/f647184fbb638f8e5a92a388ee1a6f2b.png" style="width:1.22847in;height:0.86944in" alt="倾斜传感器" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/0d81e07a0f67700c5a396fc7e1e614e1.jpeg" style="width:0.98958in;height:0.36042in" alt="3p线" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/edbfec59fe015bd9987e4b4d542b466d.png" style="width:0.8875in;height:0.47569in" alt="USB线" /></td>
</tr>
<tr class="even">
<td>ESP32 Board*1</td>
<td>ESP32 Expansion Board*1</td>
<td><p>Keyestudio</p>
<p>Tilt Sensor*1</p></td>
<td>3P Dupont Wire*1</td>
<td>Micro USB Cable*1</td>
</tr>
</tbody>
</table>

**4. Connection Diagram**

![](media/0303daa7c70c79e2e1784f9e23693425.png)

**5. Test Code**

```Python
from machine import Pin
import time

TiltSensor = Pin(15, Pin.IN)

while True:
    value = TiltSensor.value()
    print(value, end = " ")
    if  value== 0:
        print("The switch is turned on")
    else:
        print("The switch is turned off")
    time.sleep(0.1)
```


**6. Test Result**

Connect the wires according to the experimental wiring diagram and power on. Click ![](media/da852227207616ccd9aff28f19e02690.png)“Run current script”, the code starts executing, the string and the data will be displayed in the ”Shell“ window. When the tilt module is inclined to one side, the red LED on the module will be off and the Shell“ window will display“1 The switch is turned off”. In contrast, if you make it incline the other side, the red LED will light up and the monitor will display“0 The switch is turned on”, as shown below. Press “Ctrl+C”or click![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“Stop/Restart backend”to exit the program.

![](media/a08940e31dfd94613a6c5c45d94879fc.png)

### Project 9: Reed Switch Module

![](media/2a699e913fa52d9acff4b0e4a8188540.png)

**1. Overview**

In this kit, there is a Keyestudio reed switch module, which mainly uses a MKA10110 green reed component.

The reed switch is the abbreviation of the dry reed switch. It is a passive electronic switch element with contacts.

It has the advantages of simple structure, small size and easy control. Its shell is a sealed glass tube with two iron elastic reed electric plates.

In the experiment, we will determine whether there is a magnetic field near the module by reading the high and low level of the S terminal on the module; and, we display the test result in the shell.

**2. Working Principle**

In normal conditions, the glass tube in the two reeds made of special materials are separated. When a magnetic substance close to the glass tube, in the role of the magnetic field lines, the pipe within the two reeds are magnetized to attract each other in contact, the reed will suck together, so that the junction point of the connected circuit communication.

After the disappearance of the outer magnetic reed because of their flexibility and separate, the line is disconnected. The sensor uses this characteristic to build a circuit to convert magnetic field signal into high and low level signal.  

![](media/a4a9a00f86be808be0a9c784a6960cd6.jpeg)

**3. Components**

<table class="colwidths-auto docutils align-default">
<tbody>
<tr class="odd">
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/c9020c6015e55923afec197ab9d03fae.png" style="width:1.05278in;height:0.48819in" alt="4" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/6d96c844b0260ad712130945d692a7a2.jpeg" style="width:1.34444in;height:1.02986in" alt="ks0465-1" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/92c44afcc82bb13a14e8438646670cc6.png" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/0d81e07a0f67700c5a396fc7e1e614e1.jpeg" style="width:0.98958in;height:0.36042in" alt="3p线" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/edbfec59fe015bd9987e4b4d542b466d.png" style="width:0.8875in;height:0.47569in" alt="USB线" /></td>
</tr>
<tr class="even">
<td>ESP32 Board*1</td>
<td>ESP32 Expansion Board*1</td>
<td>Keyestudio DIY Reed Switch Module*1</td>
<td>3P Dupont Wire*1</td>
<td>Micro USB Cable*1</td>
</tr>
</tbody>
</table>

**4. Connection Diagram**

![](media/45cb30739b7c6518fe1591142aabbf2f.png)

**5. Test Code**


```Python
from machine import Pin
import time

ReedSensor = Pin(15, Pin.IN)
while True:
    value = ReedSensor.value()
    print(value, end = " ")
    if value == 0:
        print("A magnetic field")
    else:
        print("There is no magnetic field")
    time.sleep(0.1)
```



**6. Test Result**

Connect the wires according to the experimental wiring diagram and power on. Click ![](media/da852227207616ccd9aff28f19e02690.png)“Run current script”, the code starts executing, the string and the data will be displayed in the ”Shell“ window.

When the sensor detects a magnetic field, val is 0 and the red LED of the module lights up, "0 A magnetic field" will be displayed. When no magnetic field is detected, val is 1, and the LED on the module goes out, "1 There is no magnetic field" will be shown, as shown below. Press “Ctrl+C”or click![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“Stop/Restart backend”to exit the program.

![](media/f44214d63a5974544ca996f93764b550.png)

### Project 10: PIR Motion Sensor

![](media/d58ba7b9b4a0115b07cbb1c871ef8ec9.jpeg)

**1. Overview**

In this kit, there is a Keyestudio PIR motion sensor, which mainly uses an RE200B-P sensor elements. It is a human body pyroelectric motion sensor based on pyroelectric effect, which can detect infrared rays emitted by humans or animals, and the Fresnel lens can make the sensor's detection range farther and wider.

In the experiment, we determine if there is someone moving nearby by reading the high and low levels of the S terminal on the module. The detected results will be displayed on the Shell.

**2. Working Principle**

The upper left part is voltage conversion(VCC to 3.3V). The working voltage of sensors we use is 3.3V, therefore we can’t use 5V directly. The voltage conversion circuit is needed.

When no person is detected or no infrared signal is received, and pin 1 of the sensor outputs low level. At this time, the LED on the module will light up and the MOS tube Q1 will be connected and the signal terminal S will detect Low levels.

When one is detected or an infrared signal is received, and pin 1 of the sensor outputs a high level. Then LED on the module will go off, the MOS tube Q1 is disconnected and the signal terminal S will detect high levels.

![](media/e62f4d614ab7e67ac373576d7ff96fee.png)

**3. Required Components**

<table class="colwidths-auto docutils align-default">
<tbody>
<tr class="odd">
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/c9020c6015e55923afec197ab9d03fae.png" style="width:1.05278in;height:0.48819in" alt="4" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/6d96c844b0260ad712130945d692a7a2.jpeg" style="width:1.34444in;height:1.02986in" alt="ks0465-1" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/8712c267aff99cc16c2071398d6632af.png" style="width:1.23125in;height:0.83958in" alt="人体红外热释传感器" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/0d81e07a0f67700c5a396fc7e1e614e1.jpeg" style="width:0.98958in;height:0.36042in" alt="3p线" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/edbfec59fe015bd9987e4b4d542b466d.png" style="width:0.8875in;height:0.47569in" alt="USB线" /></td>
</tr>
<tr class="even">
<td>ESP32 Board*1</td>
<td>ESP32 Expansion Board*1</td>
<td>Keyestudio DIY PIR Motion Sensor*1</td>
<td>3P Dupont Wire*1</td>
<td>Micro USB Cable*1</td>
</tr>
</tbody>
</table>

**4. Connection Diagram**

![](media/6e57df420ca5d0dcc6f87467bb0295db.png)

**5. Test Code**

```Python
from machine import Pin
import time

PIR = Pin(15, Pin.IN)
while True:
    value = PIR.value()
    print(value, end = " ")
    if value == 1:
        print("Some body is in this area!")
    else:
        print("No one!")
    time.sleep(0.1)
```

**6. Test Result**

Connect the wires according to the experimental wiring diagram and power on. Click ![](media/da852227207616ccd9aff28f19e02690.png)“Run current script”, the code starts executing, the string and the data will be displayed in the ”Shell“ window. When the sensor detects someone nearby, value is 1, the LED will go off and the ”Shell“ window will show“1 Somebody is in this area\!”.

On the contrary, the value is 0, the LED will go up and“0 No one\!”will be shown, as shown below. Press “Ctrl+C”or click![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“Stop/Restart backend”to exit the program.

![](media/35150d4268fa4716df8624845567f888.png)

### Project 11: Active Buzzer

![](media/f4cc23dc8ed28d408e5a119855e19aa2.jpeg)

**1. Overview**

In this kit, it contains an active buzzer module and a power amplifier module (the principle is equivalent to a passive buzzer). In this experiment, we control the active buzzer to emit sounds. Since it has its own oscillating circuit, the buzzer will automatically sound if given large voltage.

**2. Working Principle**

From the schematic diagram, the pin of buzzer is connected to a resistor R2 and another port is linked with a NPN triode Q1. So, if this triode Q1 is powered, the buzzer will sound.

If the base electrode of the triode connected to the R1 resistor is a high level, the triode Q1 will be connected. If the base electrode is pulled down by the resistor R3, the triode is disconnected.

When we output a high level from the IO port to the triode, the buzzer will emit sounds; if outputting low levels, the buzzer won’t emit sounds.

![](media/458b66a2a23d6e135e7cf9975fe27507.png)

**3. Components**

<table class="colwidths-auto docutils align-default">
<tbody>
<tr class="odd">
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/c9020c6015e55923afec197ab9d03fae.png" style="width:1.05278in;height:0.48819in" alt="4" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/6d96c844b0260ad712130945d692a7a2.jpeg" style="width:1.34444in;height:1.02986in" alt="ks0465-1" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/a5e355d0fd3c9b18c7684a9a2b99f0a5.png" style="width:1.30625in;height:0.94167in" alt="有源蜂鸣器模块" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/0d81e07a0f67700c5a396fc7e1e614e1.jpeg" style="width:0.98958in;height:0.36042in" alt="3p线" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/edbfec59fe015bd9987e4b4d542b466d.png" style="width:0.8875in;height:0.47569in" alt="USB线" /></td>
</tr>
<tr class="even">
<td>ESP32 Board*1</td>
<td>ESP32 Expansion Board*1</td>
<td>Keyestudio Active Buzzer*1</td>
<td>3P Dupont Wire*1</td>
<td>Micro USB Cable*1</td>
</tr>
</tbody>
</table>

**4. Connection Diagram**

![](media/44508746060c5df3544ab2d84b2482bf.png)


**5. Test Code**


```Python
from machine import Pin
import time

buzzer = Pin(15, Pin.OUT)
while True:
    buzzer.value(1)
    time.sleep(1)
    buzzer.value(0)
    time.sleep(1)
```


**6. Code Explanation**

In the experiment, we set the pin to GPIO15. When setting to high, the active buzzer will beep. When setting to low, the active buzzer will stop emitting sounds.

**7. Test Result**

Connect the wires according to the experimental wiring diagram and power on. Click ![](media/da852227207616ccd9aff28f19e02690.png)“Run current script”, the code starts executing. The active buzzer will emit sound for 1 s, and stop for 1 s. Press “Ctrl+C”or click![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“Stop/Restart backend”to exit the program.

### Project 12: 8002b Audio Power Amplifier

![](media/6e8569df97b72e866488a6f414f9e392.jpeg)

**1. Overview**

In this kit, there is a Keyestudio 8002b audio power amplifier. The main components of this module are an adjustable potentiometer, a speaker, and an audio amplifier chip.

The main function of this module is: it can amplify the output audio signal, with a magnification of 8.5 times, and play sound or music through the built-in low-power speaker, as an external amplifying device for some music playing equipment.

In the experiment, we used the 8002b power amplifier speaker module to emit sounds of various frequencies.

**2. Working Principle**

In fact, it is similar to a passive buzzer. The active buzzer has its own oscillation source. Yet, the passive buzzer does not have internal oscillation. When controlling the circuit, we need to input square waves of different frequencies to the positive pole of the component and ground the negative pole to control the buzzer to chime sounds of different frequencies.

![](media/f5f372e0713df6439a7cc52f5caf1cad.png)

**3. Components**

<table class="colwidths-auto docutils align-default">
<tbody>
<tr class="odd">
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/c9020c6015e55923afec197ab9d03fae.png" style="width:1.05278in;height:0.48819in" alt="4" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/6d96c844b0260ad712130945d692a7a2.jpeg" style="width:1.34444in;height:1.02986in" alt="ks0465-1" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/afd2d5f63e3823e1cb941fc73a51d3ac.png" style="width:1.45556in;height:0.77986in" alt="8002b功放 喇叭模块" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/0d81e07a0f67700c5a396fc7e1e614e1.jpeg" style="width:0.98958in;height:0.36042in" alt="3p线" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/edbfec59fe015bd9987e4b4d542b466d.png" style="width:0.8875in;height:0.47569in" alt="USB线" /></td>
</tr>
<tr class="even">
<td>ESP32 Board*1</td>
<td>ESP32 Expansion Board*1</td>
<td>Keyestudio 8002b Audio Power Amplifier*1</td>
<td>3P Dupont Wire*1</td>
<td>Micro USB Cable*1</td>
</tr>
</tbody>
</table>

**4. Connection Diagram**

![](media/c6e67388d17aae690f538a4c61f9fd9f.png)

**5. Test Code**

```Python
from machine import Pin, PWM
from time import sleep
buzzer = PWM(Pin(15))

buzzer.duty(1000)

buzzer.freq(523)#DO
sleep(0.5)
buzzer.freq(586)#RE
sleep(0.5)
buzzer.freq(658)#MI
sleep(0.5)
buzzer.freq(697)#FA
sleep(0.5)
buzzer.freq(783)#SO
sleep(0.5)
buzzer.freq(879)#LA
sleep(0.5)
buzzer.freq(987)#SI
sleep(0.5)
buzzer.duty(0)
```

**6. Code Explanation**

In this experiment, we use the PWM class of the machine module, buzzer = PWM(Pin(15)) to create an instance of the PWM class, and the buzzer pin is connected to GPIO15.

The buzzer.duty(1000): set the duty cycle, and the duty cycle is 1000/4095. The larger the value, the louder the buzzer. When set to 0, the buzzer does not emit sound. **buzzer.freq()** is the frequency setting method.

In the experiment, we use the PWM on the machine module. **buzzer =PWM(Pin(15))**

**7. Test Result**

Connect the wires according to the experimental wiring diagram and power on. Click ![](media/da852227207616ccd9aff28f19e02690.png)“Run current script”, the code starts executing. The power amplifier module will emit the sound of the corresponding frequency corresponding to the beat :DO for 0.5s, Re for 0.5s, Mi for 0.5s, Fa for 0.5s, So for 0.5s, La 0.5s and Si for 0.5s. Press “Ctrl+C”or click![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“Stop/Restart backend”to exit the program.

### Project 13: Potentiometer

![](media/fe92a4f36758bc236d94290478fe5eac.jpeg)

**1. Overview**

The following we will introduce is the Keyestudio rotary potentiometer which is an analog sensor.

The digital IO ports can read the voltage value between 0 and 3.3V and the module only outputs high levels. However, the analog sensor can read the voltage value through 16 ADC analog ports on the ESP32 board. In the experiment, we will display the test results on the Shell.

**2. Working Principle**

![](media/a6ca9064a864e572984fdc41207eaaca.jpeg)

It uses a 10K adjustable resistor. We can change the resistance by rotating the potentiometer. The signal S can detect the voltage changes(0-3.3V) which are analog quantity.

**ADC：** The more bits an ADC has, the denser the partitioning of the simulation, the higher the accuracy of the final conversion.

![](media/f6c45550f4adf8373d7f1d01daec2c64.png)

Subsection 1: The analog value within 0V ~ 3.3/4095 V corresponds to the number 0;

Subsection 2: The analog value within 3.3/4095 V ~ 2*3.3/4095 V corresponds to the number 1;
 …

The conversion formula is as follows:
![Img](./media/img-20231010114044.png)

**DAC：** The higher the precision of DAC, the higher the precision of the output voltage value.  

The conversion formula is as follows:  

**ADC on ESP32：**

The ESP32 has 16 pins that can be used to measure analog signals. GPIO pin serial numbers and analog pin definitions are shown below:  

<table class="colwidths-auto docutils align-default">
<tbody>
<tr class="odd">
<td>ADC number in ESP32</td>
<td>ESP32 GPIO number</td>
</tr>
<tr class="even">
<td>ADC0</td>
<td>GPIO 36</td>
</tr>
<tr class="odd">
<td>ADC3</td>
<td>GPIO 39</td>
</tr>
<tr class="even">
<td>ADC4</td>
<td>GPIO 32</td>
</tr>
<tr class="odd">
<td>ADC5</td>
<td>GPIO33</td>
</tr>
<tr class="even">
<td>ADC6</td>
<td>GPIO34</td>
</tr>
<tr class="odd">
<td>ADC7</td>
<td>GPIO 35</td>
</tr>
<tr class="even">
<td>ADC10</td>
<td>GPIO 4</td>
</tr>
<tr class="odd">
<td>ADC11</td>
<td>GPIO0</td>
</tr>
<tr class="even">
<td>ADC12</td>
<td>GPIO2</td>
</tr>
<tr class="odd">
<td>ADC13</td>
<td>GPIO15</td>
</tr>
<tr class="even">
<td>ADC14</td>
<td>GPIO13</td>
</tr>
<tr class="odd">
<td>ADC15</td>
<td>GPIO 12</td>
</tr>
<tr class="even">
<td>ADC16</td>
<td>GPIO 14</td>
</tr>
<tr class="odd">
<td>ADC17</td>
<td>GPIO27</td>
</tr>
<tr class="even">
<td>ADC18</td>
<td>GPIO25</td>
</tr>
<tr class="odd">
<td>ADC19</td>
<td>GPIO26</td>
</tr>
</tbody>
</table>

**DAC on ESP32：**

The ESP32 has two 8-bit digital-to-analog converters connected to GPIO25 and GPIO26 pins, which are immutable, as shown below :

<table class="colwidths-auto docutils align-default">
<tbody>
<tr class="odd">
<td>Simulate pin number</td>
<td>GPIO number</td>
</tr>
<tr class="even">
<td>DAC1</td>
<td>GPIO25</td>
</tr>
<tr class="odd">
<td>DAC2</td>
<td>GPIO26</td>
</tr>
</tbody>
</table>

**3. Components**

<table class="colwidths-auto docutils align-default">
<tbody>
<tr class="odd">
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/c9020c6015e55923afec197ab9d03fae.png" style="width:1.05278in;height:0.48819in" alt="4" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/6d96c844b0260ad712130945d692a7a2.jpeg" style="width:1.34444in;height:1.02986in" alt="ks0465-1" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/9d866a71104fb3cf1826c41c3c940ba8.png" style="width:1.25in;height:0.86667in" alt="旋转电位器传感器" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/0d81e07a0f67700c5a396fc7e1e614e1.jpeg" style="width:0.98958in;height:0.36042in" alt="3p线" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/edbfec59fe015bd9987e4b4d542b466d.png" style="width:0.8875in;height:0.47569in" alt="USB线" /></td>
</tr>
<tr class="even">
<td>ESP32 Board*1</td>
<td>ESP32 Expansion Board*1</td>
<td>Keyestudio Rotary Potentiometer*1</td>
<td>3P Dupont Wire*1</td>
<td>Micro USB Cable*1</td>
</tr>
</tbody>
</table>

**4. Connection Diagram**

![](media/ce7b953cd508fd8f2f9aafb805fae1f6.png)

**5. Test Code**


```Python
# Import Pin, ADC and DAC modules.
from machine import ADC,Pin,DAC
import time

# Turn on and configure the ADC with the range of 0-3.3V 
adc=ADC(Pin(34))
adc.atten(ADC.ATTN_11DB)
adc.width(ADC.WIDTH_12BIT)

# Read ADC value once every 0.1seconds, convert ADC value to DAC value and output it,
# and print these data to “Shell”. 
try:
    while True:
        adcVal=adc.read()
        dacVal=adcVal//16
        voltage = adcVal / 4095.0 * 3.3
        print("ADC Val:",adcVal,"DACVal:",dacVal,"Voltage:",voltage,"V")
        time.sleep(0.1)
except:
    pass
```


**6. Code Explanation**

In the experiment, add "From Machine import ADC" to the top of your Python file every time you use the ACD module, the same goes for DAC modules. 

**machine.ADC(pin):** Create an ADC object associated with the given pin.
**pin：** The available pins are Pin(36)、Pin(39)、Pin(34）、Pin(35)、Pin(32)、Pin(33). 

**DAC(pin):** Create an DAC object associated with the given pin. Pin：The available pins are pin (25) 、pin (26).

**ADC. Read():** Read ADC value and return ADC value.  

**ADC.atten(db):** Set attenuation ration (that is, the full range voltage, such as the voltage of 11db full range is 3.3V)

**db：** attenuation ratio

**ADC.ATTIN\_0DB** —full range of 1.2V

**ADC.ATTN\_2\_5\_DB** —full range of 1.5V

**ADC.ATTN\_6DB** —full range of 2.0 V

**ADC.ATTN\_11DB** —full range of 3.3V

**ADC.width(bit):** Set data width.

**bit：** data bit

**ADC.WIDTH\_9BIT** —9 data width

**ADC.WIDTH\_10BIT** — 10 data width

**ADC.WIDTH\_11BIT** — 11 data width

**ADC.WIDTH\_12BIT** — 12 data width

**The read()method reads the** ADCvalue，rang is 0\~4095，the **adc.read()** reads the ADC value input by the ADC(Pin(34)) Pin and assigns it to a variable named adcVal.  

**DAC.write(value):** Output the voltage value, the data rang : 0-255，the corresponding output voltage is 0-3.3V.

**7. Test Result**

Connect the wires according to the experimental wiring diagram and power on. Click ![](media/da852227207616ccd9aff28f19e02690.png)“Run current script”, the code starts executing. The "Shell" window prints and displays the potentiometer ADC value, DAC value and voltage value. Rotating the potentiometer handle, the ADC value, DAC value and voltage value will change. Press “Ctrl+C”or click![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“Stop/Restart backend”to exit the program.

![](media/65e6848785b8e09c731df4dd1f68a3a0.png)

### Project 14: Sound Sensor

![](media/c4d4961f71c7e91bae04507f72cb56eb.jpeg)

**1. Overview**

In this kit, there is a Keyestudio DIY electronic block and a sound sensor. In the experiment, we test the analog value corresponding to the sound level in the current environment with it. The louder the sound, the larger the ADC, DAC and the voltage value, and the “shell” window will display the test results.

**2. Working Principle**

It uses a high-sensitive microphone component and an LM386 chip. We build the circuit with the LM386 chip and amplify the sound through the high-sensitive microphone. In addition, we can adjust the sound volume by the potentiometer. Rotate it clockwise, the sound will get louder.

![](media/d55fc5234be47e7727c0bf48c049e341.jpeg)

**3. Components**

<table class="colwidths-auto docutils align-default">
<tbody>
<tr class="odd">
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/c9020c6015e55923afec197ab9d03fae.png" style="width:1.05278in;height:0.48819in" alt="4" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/6d96c844b0260ad712130945d692a7a2.jpeg" style="width:1.34444in;height:1.02986in" alt="ks0465-1" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/6406b86b355b4986a8b2ec74f770c2ba.png" style="width:1.19167in;height:0.92292in" alt="声音传感器" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/0d81e07a0f67700c5a396fc7e1e614e1.jpeg" style="width:0.98958in;height:0.36042in" alt="3p线" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/edbfec59fe015bd9987e4b4d542b466d.png" style="width:0.8875in;height:0.47569in" alt="USB线" /></td>
</tr>
<tr class="even">
<td>ESP32 Board*1</td>
<td>ESP32 Expansion Board*1</td>
<td>Keyestudio DIY Sound Sensor*1</td>
<td>3P Dupont Wire*1</td>
<td>Micro USB Cable*1</td>
</tr>
</tbody>
</table>

**4. Connection Diagram**

![](media/7a5b741aba98560eddadc3b7788325d9.png)

**5. Test Code**

```Python
# Import Pin, ADC and DAC modules.
from machine import ADC,Pin,DAC
import time

# Turn on and configure the ADC with the range of 0-3.3V 
adc=ADC(Pin(34))
adc.atten(ADC.ATTN_11DB)
adc.width(ADC.WIDTH_12BIT)

# Read ADC value once every 0.1seconds, convert ADC value to DAC value and output it,
# and print these data to “Shell”. 
try:
    while True:
        adcVal=adc.read()
        dacVal=adcVal//16
        voltage = adcVal / 4095.0 * 3.3
        print("ADC Val:",adcVal,"DACVal:",dacVal,"Voltage:",voltage,"V")
        time.sleep(0.1)
except:
    pass
```


**6. Test Result**

Connect the wires according to the experimental wiring diagram and power on. Click ![](media/da852227207616ccd9aff28f19e02690.png)“Run current script”, the code starts executing. The "Shell" window will display the sound sensor ADC value, DAC value and voltage value. Rotate the potentiometer clockwise and speak at the MIC. Then you can see the analog value get larger, as shown below. Press “Ctrl+C”or click![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“Stop/Restart backend”to exit the program.

![](media/16c179e59bfbbb62544d74ce501f0aa2.png)

### Project 15: Photoresistor

![](media/37bb57bcf72ba62056bbc61164185f0a.png)

**1. Description**

In this kit, there is a photoresistor which consists of photosensitive resistance elements. Its resistance changes with the light intensity. Also, it converts the resistance change into a voltage change through the characteristic of the photosensitive resistive element. When wiring it up, we interface its signal terminal (S terminal) with the analog port of ESP32 , so as to sense the change of the analog value, and display the corresponding analog value in the shell.

**2. Working Principle**

If there is no light, the resistance is 0.2MΩ and the detected voltage at the signal terminal is close to 0. When the light intensity increases, the resistance of photoresistor and detected voltage will diminish and the detected voltage will increase. 

![](media/651e70e24ecca152ec701deb7a6ea102.png)

**3. Components**

<table class="colwidths-auto docutils align-default">
<tbody>
<tr class="odd">
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/c9020c6015e55923afec197ab9d03fae.png" style="width:1.05278in;height:0.48819in" alt="4" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/6d96c844b0260ad712130945d692a7a2.jpeg" style="width:1.34444in;height:1.02986in" alt="ks0465-1" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/21847f439e9532462a71d11921112a66.png" style="width:1.12222in;height:0.82986in" alt="光敏电阻传感器" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/0d81e07a0f67700c5a396fc7e1e614e1.jpeg" style="width:0.98958in;height:0.36042in" alt="3p线" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/edbfec59fe015bd9987e4b4d542b466d.png" style="width:1.18819in;height:0.63681in" alt="USB线" /></td>
</tr>
<tr class="even">
<td>ESP32 Board*1</td>
<td>ESP32 Expansion Board*1</td>
<td>Keyestudio DIY Photoresistor*1</td>
<td>3P Dupont Wire*1</td>
<td>Micro USB Cable*1</td>
</tr>
</tbody>
</table>

**4. Connection Diagram**

![](media/0b880c099cb70864881c501c9a3a8dbb.png)

**5. Test Code**


```Python
# Import Pin, ADC and DAC modules.
from machine import ADC,Pin,DAC
import time

# Turn on and configure the ADC with the range of 0-3.3V 
adc=ADC(Pin(34))
adc.atten(ADC.ATTN_11DB)
adc.width(ADC.WIDTH_12BIT)

# Read ADC value once every 0.1seconds, convert ADC value to DAC value and output it,
# and print these data to “Shell”. 
try:
    while True:
        adcVal=adc.read()
        dacVal=adcVal//16
        voltage = adcVal / 4095.0 * 3.3
        print("ADC Val:",adcVal,"DACVal:",dacVal,"Voltage:",voltage,"V")
        time.sleep(0.1)
except:
    pass
```


**6. Test Result**

Connect the wires according to the experimental wiring diagram and power on. Click ![](media/da852227207616ccd9aff28f19e02690.png)“Run current script”, the code starts executing. The "Shell" window will display the photoresistor ADC value, DAC value and voltage value. The brighter the light, the greater the analog value, as shown below. Press “Ctrl+C”or click![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“Stop/Restart backend”to exit the program.

![](media/3b141ec51733d34caff4f0b2afc653a4.png)

### Project 16: NTC-MF52AT Thermistor

![](media/868d93395d983645baab872091991403.jpeg)

**1. Overview**

In the experiment, there is a NTC-MF52AT analog thermistor. We connect its signal terminal to the analog port of the ESP32 mainboard and read the corresponding ADC value, voltage value and thermistor value.

We can use analog values to calculate the temperature of the current environment through specific formulas. Since the temperature calculation formula is more complicated, we only read the corresponding analog value.

**2. Working Principle**

![](media/84a67bb2b90b4740c09d914dc6402f48.png)

This module mainly uses NTC-MF52AT thermistor element, which can sense the changes of the surrounding environment temperature. Resistance changes with the temperature, causing the voltage of the signal terminal S to change.

This sensor uses the characteristics of NTC-MF52AT thermistor element to convert resistance changes into voltage changes.

**3. Components**

<table class="colwidths-auto docutils align-default">
<tbody>
<tr class="odd">
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/c9020c6015e55923afec197ab9d03fae.png" style="width:1.05278in;height:0.48819in" alt="4" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/6d96c844b0260ad712130945d692a7a2.jpeg" style="width:1.34444in;height:1.02986in" alt="ks0465-1" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/481d8a887573a4aeeb9a61a8f5b1fe6f.png" style="width:1.24236in;height:0.83889in" alt="模拟温度传感器" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/0d81e07a0f67700c5a396fc7e1e614e1.jpeg" style="width:0.98958in;height:0.36042in" alt="3p线" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/edbfec59fe015bd9987e4b4d542b466d.png" style="width:1.18819in;height:0.63681in" alt="USB线" /></td>
</tr>
<tr class="even">
<td>ESP32 Board*1</td>
<td>ESP32 Expansion Board*1</td>
<td>Keyestudio NTC-MF52AT Thermistor*1</td>
<td>3P Dupont Wire*1</td>
<td>Micro USB Cable*1</td>
</tr>
</tbody>
</table>

**4. Connection Diagram**

![](media/7fba5e360e5bcc3e60ef27a77b3362d1.png)

**5. Test Code**


```Python
from machine import Pin, ADC
import time
import math

#Set ADC
adc=ADC(Pin(34))
adc.atten(ADC.ATTN_11DB)
adc.width(ADC.WIDTH_12BIT)

try:
    while True:
        adcValue = adc.read()
        voltage = adcValue / 4095 * 3.3
        Rt = 4.7 *  (3.3-voltage)/voltage 
        tempK = (1 / (1 / (273.15+25) + (math.log(Rt/10)) / 3950))
        tempC = (tempK - 273.15)
        print("ADC value:",adcValue,"  Voltage:",voltage,"V","  Temperature: ",tempC,"C");
        time.sleep(1)
except:
    pass
```


**6. Test Result**

Connect the wires according to the experimental wiring diagram and power on. Click ![](media/da852227207616ccd9aff28f19e02690.png)“Run current script”, the code starts executing. The "Shell" window will display the thermistor ADC value, voltage value and temperature value, as shown below. Press “Ctrl+C”or click![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“Stop/Restart backend”to exit the program.

![](media/77f18a9e099306cd7111d6b2df2b5eb6.png)

### Project 17: Thin-film Pressure Sensor

![](media/a9ae2963fc87b3502703f7dd5eb208ec.jpeg)

**1. Overview**

In this kit, there is a Keyestudio thin-film pressure sensor. The thin-film pressure sensor composed of a new type of nano pressure-sensitive material and a comfortable ultra-thin film substrate, has waterproof and pressure-sensitive functions.

In the experiment, we determine the pressure by collecting the analog signal on the S end of the module. The smaller the ADC value, DAC value and voltage value, the greater the pressure; and the displayed results will shown on the Shell.

**2. Working Principle**

When the sensor is pressed by external forces, the resistance value of sensor will vary. We convert the pressure signals detected by the sensor into the electric signals through a circuit. Then we can obtain the pressure changes by detecting voltage signal changes.
![](media/520fa537602873d2a337731318668348.png)

**3. Components**

<table class="colwidths-auto docutils align-default">
<tbody>
<tr class="odd">
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/c9020c6015e55923afec197ab9d03fae.png" style="width:1.05278in;height:0.48819in" alt="4" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/6d96c844b0260ad712130945d692a7a2.jpeg" style="width:1.34444in;height:1.02986in" alt="ks0465-1" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/84d460c90f09b3f3baa5819ab8655e87.png" style="width:0.375in;height:1.21042in" alt="薄膜压力传感器" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/0d81e07a0f67700c5a396fc7e1e614e1.jpeg" style="width:0.98958in;height:0.36042in" alt="3p线" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/edbfec59fe015bd9987e4b4d542b466d.png" style="width:1.18819in;height:0.63681in" alt="USB线" /></td>
</tr>
<tr class="even">
<td>ESP32 Board*1</td>
<td>ESP32 Expansion Board*1</td>
<td><p>Keyestudio</p>
<p>Thin-film Pressure Sensor*1</p></td>
<td>3P Dupont Wire*1</td>
<td>Micro USB Cable*1</td>
</tr>
</tbody>
</table>

**4. Connection Diagram**

![](media/a461b6b0227b4430b64da6e80be8d898.png)

**5. Test Code**


```Python
# Import Pin, ADC and DAC modules.
from machine import ADC,Pin,DAC
import time

# Turn on and configure the ADC with the range of 0-3.3V 
adc=ADC(Pin(34))
adc.atten(ADC.ATTN_11DB)
adc.width(ADC.WIDTH_12BIT)

# Read ADC value once every 0.1seconds, convert ADC value to DAC value and output it,
# and print these data to “Shell”. 
try:
    while True:
        adcVal=adc.read()
        dacVal=adcVal//16
        voltage = adcVal / 4095.0 * 3.3
        print("ADC Val:",adcVal,"DACVal:",dacVal,"Voltage:",voltage,"V")
        time.sleep(0.1)
except:
    pass
```

**6. Test Result**

Connect the wires according to the experimental wiring diagram and power on. Click ![](media/da852227207616ccd9aff28f19e02690.png)“Run current script”, the code starts executing. The "Shell" window will display the thin-film pressure sensor ADC value, voltage value and DAC value. When the thin-film is pressed by fingers, the analog value will decrease, as shown below. Press “Ctrl+C”or click![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“Stop/Restart backend” to exit the program.

![](media/e43fa7aaed34eea4fee5a535699ddf3f.png)

### Project 18: Joystick Module

![](media/a28a09d0d9103cc8b93f2ae71f98482a.jpeg)

**1. Overview**

Game handle controllers are ubiquitous.

It mainly uses PS2 joysticks. When controlling it, we need to connect the X and Y ports of the module to the analog port of the single-chip microcomputer, port B to the digital port of the single-chip microcomputer, VCC to the power output port(3.3-5V), and GND to the GND of the MCU. We can read the high and low levels of two analog values and one digital port) to determine the working status of the joystick on the module.

In the experiment, two analog values(x axis and y axis) will be shown on Shell.

![](media/d037d9366b6094d674588c9be05aeb19.png)

**2. Working Principle**

In fact, its working principle is very simple. Its inside structure is equivalent to two adjustable potentiometers and a button. When this button is not pressed and the module is pulled down by R1, low levels will be output ; on the contrary, when the button is pressed, VCC will be connected (high levels). When we move the joystick, the internal potentiometer will adjust to output different voltages, and we can read the analog value.

**3. Components**

<table class="colwidths-auto docutils align-default">
<tbody>
<tr class="odd">
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/c9020c6015e55923afec197ab9d03fae.png" style="width:1.05278in;height:0.48819in" alt="4" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/6d96c844b0260ad712130945d692a7a2.jpeg" style="width:1.34444in;height:1.02986in" alt="ks0465-1" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/1f5bf5d8d48c675b98dd2cbfca6c31b7.png" style="width:1.38819in;height:0.73681in" alt="摇杆模块" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/fc3fd9c0110b04d1af77a2ff8c01a10a.png" style="width:0.95208in;height:0.39861in" alt="5p线" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/edbfec59fe015bd9987e4b4d542b466d.png" style="width:1.18819in;height:0.63681in" alt="USB线" /></td>
</tr>
<tr class="even">
<td>ESP32 Board*1</td>
<td>ESP32 Expansion Board*1</td>
<td>Keyestudio Joystick Module*1</td>
<td>5P Dupont Wire*1</td>
<td>Micro USB Cable*1</td>
</tr>
</tbody>
</table>

**4. Connection Diagram**

![](media/c1838e7013bc930e997d7684229bcea3.png)

**5. Test Code**


```Python
from machine import Pin, ADC
import time
# Initialize the joystick module (ADC function)
rocker_x=ADC(Pin(34)) 
rocker_y=ADC(Pin(35))
button_z=Pin(13,Pin.IN,Pin.PULL_UP)

# Set the acquisition range of voltage of the two ADC channels to 0-3.3V,
# and the acquisition width of data to 0-4095.
rocker_x.atten(ADC.ATTN_11DB)
rocker_y.atten(ADC.ATTN_11DB)
rocker_x.width(ADC.WIDTH_12BIT)
rocker_y.width(ADC.WIDTH_12BIT)
 
# In the code, configure Z_Pin to pull-up input mode.
# In loop(), use Read () to read the value of axes X and Y 
# and use value() to read the value of axis Z, and then display them.
while True:
    print("X,Y,Z:",rocker_x.read(),",",rocker_y.read(),",",button_z.value())
    time.sleep(0.5)
```




**6. Code Explanation**

In the experiment, according to the wiring diagram, the x pin is set to GPIO34, the y pin is set to GPIO35 and the pin of the joystick is set to GPIO13.

**7. Test Result**

Wiring up and powering on, then click ![](media/da852227207616ccd9aff28f19e02690.png)“Run current script”, the code starts executing. The "Shell" window will print the analog and digital values of the current joystick. Moving the joystick or pressing it will change the analog and digital values in "Shell". Press“Ctrl+C”or click![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“Stop/Restart backend”to exit the program.

![](media/06a9de681779df5cfc7e6bc24a928a3a.jpeg)

![](media/6e7dd18099836222c5237c9e0e659539.png)

### Project 19: SK6812 RGB Module

![](media/effda831f7c06cea2c443d8352f1a693.jpeg)

**1. Overview**

In previous lessons, we learned about the plug-in RGB module and used PWM signals to color the three pins of the module.

There is a Keyestudio 6812 RGB module whose the driving principle is different from the plug-in RGB module. It can only control with one pin. This is a set. It is an intelligent externally controlled LED light source with the control circuit and the light-emitting circuit. Each LED element is the same as a 5050 LED lamp bead, and each component is a pixel. There are four lamp beads on the module, which indicates four pixels.

In the experiment, we make different lights show different colors.

**2. Working Principle**

From the schematic diagram, we can see that these four pixel lighting beads are all connected in series. In fact, no matter how many they are, we can use a pin to control a light and let it display any color. The pixel point contains a data latch signal shaping amplifier drive circuit, a high-precision internal oscillator and a 12V high-voltage programmable constant current control part, which effectively ensures the color of the pixel point light is highly consistent.

The data protocol adopts a single-wire zero-code communication method. After the pixel is powered up and reset, the S terminal receives the data transmitted from the controller. The first 24bit data sent is extracted by the first pixel and sent to the data latch of the pixel.

![](media/f0d824a10a88aa0fbabfb685634672fc.png)

**3. Components**

<table class="colwidths-auto docutils align-default">
<tbody>
<tr class="odd">
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/c9020c6015e55923afec197ab9d03fae.png" style="width:1.05278in;height:0.48819in" alt="4" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/6d96c844b0260ad712130945d692a7a2.jpeg" style="width:1.34444in;height:1.02986in" alt="ks0465-1" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/42e093202e7233aaaa42b9ac64f51d98.png" style="width:1.26111in;height:0.875in" alt="6812 RGB模块" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/0d81e07a0f67700c5a396fc7e1e614e1.jpeg" style="width:0.98958in;height:0.36042in" alt="3p线" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/edbfec59fe015bd9987e4b4d542b466d.png" style="width:1.18819in;height:0.63681in" alt="USB线" /></td>
</tr>
<tr class="even">
<td>ESP32 Board*1</td>
<td>ESP32 Expansion Board*1</td>
<td>Keyestudio 6812 RGB Module*1</td>
<td>3P Dupont Wire*1</td>
<td>Micro USB Cable*1</td>
</tr>
</tbody>
</table>

**4. Connection Diagram**

![](media/c24ec4320937c7115802a2937180f703.png)

**5. Test Code**


```Python
#Import Pin, neopiexl and time modules.
from machine import Pin
import neopixel
import time

#Define the number of pin and LEDs connected to neopixel.
pin = Pin(15, Pin.OUT)
np = neopixel.NeoPixel(pin, 4) 

#brightness :0-255
brightness=100                                
colors=[[brightness,0,0],                    #red
        [0,brightness,0],                    #green
        [0,0,brightness],                    #blue
        [brightness,brightness,brightness],  #white
        [0,0,0]]                             #close

#Nest two for loops to make the module repeatedly display five states of red, green, blue, white and OFF.    
while True:
    for i in range(0,5):
        for j in range(0,4):
            np[j]=colors[i]
            np.write()
            time.sleep_ms(50)
        time.sleep_ms(500)
    time.sleep_ms(500)
```





**6. Code Explanation**

A few function ports and functions:

**np = neopixel.NeoPixel(pin, 4)** , there are four LED beads, so we set to 4.

**pin = Pin(15, Pin.OUT)** , this is the pin number, we connect to GP15.

**brightness = 100**, brightness setting 255 implies brightest.

**7. Test Result**

Connect the wires according to the experimental wiring diagram and power on. Click ![](media/da852227207616ccd9aff28f19e02690.png)“Run current script”, the code starts executing.  Then we can see the four RGB LEDs show different colors.

Press “Ctrl+C”or click![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“Stop/Restart backend”to exit the program.

### Project 20: Rotary Encoder

![](media/ec37b336b8f5620b62b04224b132840a.jpeg)

**1. Overview**

In this kit, there is a Keyestudio rotary encoder, dubbed as switch encoder. It is applied to automotive electronics, multimedia audio, instrumentation, household appliances, smart home, medical equipment and so on.

In the experiment, it it used for counting. When we rotate the rotary encoder clockwise, the set data falls by 1. If you rotate it anticlockwise, the set data is up 1, and when the middle button is pressed, the value will be show on Shell.

**2. Working Principle**

The incremental encoder converts the displacement into a periodic electric signal, and then converts this signal into a counting pulse, and the number of pulses indicates the size of the displacement.This module mainly uses 20pulse rotary encoder components. It can calculate the number of pulses output during clockwise and reverse rotation. There is no limit to count rotation. It resets to the initial state, that is, starts counting from 0.           

![](media/2fb56ec6fa69e66fcca4243617d4b18c.jpeg)

**3. Components**

<table class="colwidths-auto docutils align-default">
<tbody>
<tr class="odd">
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/c9020c6015e55923afec197ab9d03fae.png" style="width:1.05278in;height:0.48819in" alt="4" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/6d96c844b0260ad712130945d692a7a2.jpeg" style="width:1.34444in;height:1.02986in" alt="ks0465-1" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/989ee8ccd2a016dcaeb0bef68d55e912.png" style="width:1.27708in;height:0.73264in" alt="旋转编码器模块" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/fc3fd9c0110b04d1af77a2ff8c01a10a.png" style="width:0.95208in;height:0.39861in" alt="5p线" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/edbfec59fe015bd9987e4b4d542b466d.png" style="width:0.94653in;height:0.41806in" alt="USB线" /></td>
</tr>
<tr class="even">
<td>ESP32 Board*1</td>
<td>ESP32 Expansion Board*1</td>
<td>Keyestudio Rotary Encoder*1</td>
<td>5P Dupont Wire*1</td>
<td>Micro USB Cable*1</td>
</tr>
</tbody>
</table>

**4. Connection Diagram**

![](media/add429af09e0e3d449fba9b17b3d0af4.png)

**5. Add Library**

Open“Thonny”，click“This computer”→“D:”→“2. ESP32\_code\_MicroPython”→“lesson 30. Rotary encoder counting”. Select“<span style="color: rgb(255, 76, 65);">rotary\.py</span>”and“<span style="color: rgb(255, 76, 65);">rotary\_irq\_rp2.py</span>”，right-click“<span style="color: rgb(255, 76, 65);">Upload to /</span>”.

![Img](./media/img-20231010115621.png)
![Img](./media/img-20231010115626.png)


**6. Test Code**


```Python
import time
from rotary_irq_rp2 import RotaryIRQ
from machine import Pin

SW=Pin(27,Pin.IN,Pin.PULL_UP)  
r = RotaryIRQ(pin_num_clk=12,
              pin_num_dt=14,
              min_val=0,
              reverse=False,
              range_mode=RotaryIRQ.RANGE_UNBOUNDED)
val_old = r.value()
while True:
    try:
        val_new = r.value()
        if SW.value()==0 and n==0:
            print("Button Pressed")
            print("Selected Number is : ",val_new)
            n=1
            while SW.value()==0:
                continue
        n=0
        if val_old != val_new:
            val_old = val_new
            print('result =', val_new)
        time.sleep_ms(50)
    except KeyboardInterrupt:
        break
```






**7. Code Explanation**

1). We will see the file **rotary\.py** and **rotary\_irq\_rp2.py**. This means that we save them in the ESP32 successfully. Then we can use **from rotary\_irq\_rp2 import RotaryIRQ.**
    
2). **SW=Pin(27,Pin.\IN, Pin.PULL\_UP)** indicates that the SW pin is connected to GPIO27, **pin\_num\_clk=12** indicates that the pin CLK is connected to GPIO12, and **pin\_num\_dt=14** means that the DT pin is connected to GPIO14. We can change these pin numbers.
    
3). **try/except** is the python language exception capture processing statement, **try** executes the code, **except** executes the code, when an exception occurs, and when we press Ctrl+C, the program exits.
    
4). **r.value()** returns the value of the encoder

**8. Test Result**

Connect the wires according to the experimental wiring diagram and power on. Click ![](media/da852227207616ccd9aff28f19e02690.png)“Run current script”, the code starts executing. Rotate the encoder clockwise, the displayed data will decrease, rotate the encoder counterclockwise, the displayed data will increase. Press the middle button of the encoder, the displayed data is the value of the encoder, as shown in the figure below. Press “Ctrl+C”or click![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“Stop/Restart backend”to exit the program.

![](media/ea0e88b6a555f4dff831966f20c89782.png)

### Project 21: Servo Control

![](media/165f16e47a832fc4dcaea6e4a1c11194.jpeg)

**1. Overview**

Servo is a position control rotary actuator. It mainly consists of a housing, a circuit board, a core-less motor, a gear and a position sensor. 

In general, servo has three lines in brown, red and orange. The brown wire is grounded, the red one is a positive pole line and the orange one is a signal line.

![](media/3366fe332bcf286659f9bf21a8cf880f.png)

**2. Working Principle**

The rotation angle of servo motor is controlled by regulating the duty cycle of PWM (Pulse-Width Modulation) signal. The standard cycle of PWM signal is 20ms (50Hz). Theoretically, the width is distributed between 1ms-2ms, but in fact, it's between 0.5ms-2.5ms. The width corresponds the rotation angle from 0° to 180°. But note that for different brand motors, the same signal may have different rotation angles. 

![](media/b4993212773e13b1a4424b3d7ef41ab6.png)

**3. Components**

<table class="colwidths-auto docutils align-default">
<tbody>
<tr class="odd">
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/c9020c6015e55923afec197ab9d03fae.png" style="width:1.05278in;height:0.48819in" alt="4" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/6d96c844b0260ad712130945d692a7a2.jpeg" style="width:1.34444in;height:1.02986in" alt="ks0465-1" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/b9a96e60ed3aee985db5d4dcaf9bf38b.png" style="width:1.05764in;height:1.25in" alt="舵机" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/edbfec59fe015bd9987e4b4d542b466d.png" style="width:1.18819in;height:0.63681in" alt="USB线" /></td>
</tr>
<tr class="even">
<td>ESP32 Board*1</td>
<td>ESP32 Expansion Board*1</td>
<td>Servo*1</td>
<td>Micro USB Cable*1</td>
</tr>
</tbody>
</table>

**4. Connection Diagram**

![](media/53dbdf43b364542bedb39e45132a2af9.png)

**5. Test Code 1**

```Python
from machine import Pin, PWM
import time
pwm = PWM(Pin(4))  
pwm.freq(50)

'''
Duty cycle corresponding to the Angle
0°----2.5%----25
45°----5%----51.2
90°----7.5%----77
135°----10%----102.4
180°----12.5%----128
'''
angle_0 = 25
angle_90 = 77
angle_180 = 128

while True:
    pwm.duty(angle_0)
    time.sleep(1)
    pwm.duty(angle_90)
    time.sleep(1)
    pwm.duty(angle_180)
    time.sleep(1)
```


**6. Code Explanation 1**

According to the angle of the signal pulse width, it is converted into a duty cycle. The formula is: 2.5+angle/180\*10. The PWM pin resolution of ESP32 is 2^10 = 1024. When converted to 0 degree, its duty cycle is 1024* 2.5% = 25.6 , when the angle is 180 degrees, its duty cycle value is 1024\* 12.5% = 128, these two values will be related to the program, considering the error and rotation angle, I set the duty cycle at between 10 and 150, the servo can rotate smoothly 0\~180 degrees.

**7. Test Result 1**

Connect the wires according to the experimental wiring diagram and power on. Click ![](media/da852227207616ccd9aff28f19e02690.png)“Run current script”, the code starts executing, the servo will rotate 0°，90° and 180° cyclically. Press “Ctrl+C”or click![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“Stop/Restart backend” to exit the program.

**8. Test Code 2**


```Python
from utime import sleep
from machine import Pin
from machine import PWM

pwm = PWM(Pin(4))#Steering gear pin is connected to GP4.
pwm.freq(50)#20ms period, so the frequency is 50Hz
'''
Duty cycle corresponding to the Angle
0°----2.5%----25
45°----5%----51.2
90°----7.5%----77
135°----10%----102.4
180°----12.5%----128
'''
# Set the servo motor rotation Angle
def setServoCycle (position):
    pwm.duty(position)
    sleep(0.01)

# Convert the rotation Angle to duty cycle
def convert(x, i_m, i_M, o_m, o_M):
    return max(min(o_M, (x - i_m) * (o_M - o_m) // (i_M - i_m) + o_m), o_m)

while True:
    for degree in range(0, 180, 1):#servo goes from 0 to 180
        pos = convert(degree, 0, 180, 20, 150)
        setServoCycle(pos)

    for degree in range(180, 0, -1):#servo goes from 180 to 0
        pos = convert(degree, 0, 180, 20, 150)
        setServoCycle(pos)
```




**9. Code Explanation 2**

**convert(x, i\_m, i\_M, o\_m, o\_M)**: x is the value we want to map;
**i\_m, i\_M** are the lower and upper limits of the current value;
**o\_m, o\_M** are the lower and upper limits of the target range we want to map to.

**10. Test Result 2**

Connect the wires according to the experimental wiring diagram and power on. Click ![](media/da852227207616ccd9aff28f19e02690.png)“Run current script”, the code starts executing. The servo rotates from 0° to 180° by moving 1° for each 15ms. Press “Ctrl+C”or click![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“Stop/Restart backend”to exit the program.

### Project 22: Ultrasonic Sensor

![](media/8f99fc89502d1ae2543839b4950da5b6.jpeg)

Bats and some marine animals are able to use high frequencies of sound for echolocation or communication. They can emit ultrasonic waves from the larynx through the mouth or nose and use the sound waves that bounce back to orient and determine the position, size and whether nearby objects are moving.

Ultrasonic is a frequency higher than 20000 Hz sound wave, which has a good direction, a strong penetration ability, and is easy to obtain more concentrated sound energy as well as spread far in the water. It can be used for ranging, speed measurement, cleaning, welding, gravel, sterilization and disinfection. What‘s more, it has many applications in medicine, military, industry and agriculture.

**1. Overview**

In this kit, there is a keyes HC-SR04 ultrasonic sensor, which can detect obstacles in front and the detailed distance between the sensor and the obstacle. Its principle is the same as that of bat flying. It can emit the ultrasonic signals that cannot be heard by humans. When these signals hit an obstacle and come back immediately. The distance between the sensor and the obstacle can be calculated by the time gap of emitting signals and receiving signals.

In the experiment, we use the sensor to detect the distance between the sensor and the obstacle, and print the test result.

**2. Working Principle**

The most common ultrasonic ranging method is the echo detection. As shown below; when the ultrasonic emitter emits the ultrasonic waves towards certain direction, the counter will count. The ultrasonic waves travel and reflect back once encountering the obstacle. Then the counter will stop counting when the receiver receives the ultrasonic waves coming back.

The ultrasonic wave is also sound wave, and its speed of sound V is related to temperature. Generally, it travels 340m/s in the air. According to time t, we can calculate the distance s from the emitting spot to the obstacle.

s=340t/2.

The HC-SR04 ultrasonic ranging module can provide a non-contact distance sensing function of 2cm-400cm, and the ranging accuracy can reach as high as 3mm; the module includes an ultrasonic transmitter, receiver and control circuit. Basic working principle:

1). First pull down the TRIG, and then trigger it with at least 10us high level signal;

2). After triggering, the module will automatically transmit eight 40KHZ square waves, and automatically detect whether there is a signal to return.

3). If there is a signal returned back, through the ECHO to output a high level, the duration time of high level is actually the time from emission to reception of ultrasonic.

![](media/686176f637ba288e3b20d63bb1054477.png)

**3. Components**

<table class="colwidths-auto docutils align-default">
<tbody>
<tr class="odd">
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/c9020c6015e55923afec197ab9d03fae.png" style="width:1.05278in;height:0.48819in" alt="4" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/6d96c844b0260ad712130945d692a7a2.jpeg" style="width:1.34444in;height:1.02986in" alt="ks0465-1" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/1a1dc36771654248ade08b9d9f115f57.png" style="width:1.42292in;height:0.80903in" alt="超声波模块" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/269c154eda332be03643bada56070124.jpeg" style="width:0.91458in;height:0.35625in" alt="4p线" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/edbfec59fe015bd9987e4b4d542b466d.png" style="width:1.18819in;height:0.63681in" alt="USB线" /></td>
</tr>
<tr class="even">
<td>ESP32 Board*1</td>
<td>ESP32 Expansion Board*1</td>
<td>keyestudio SR01 Ultrasonic Sensor*1</td>
<td>4P Dupont Wire*1</td>
<td>Micro USB Cable*1</td>
</tr>
</tbody>
</table>

**4. Connection Diagram**

![](media/07eb56920ed1cb9b55deab51b7c61d8d.png)

**5. Test Code**


```Python
from machine import Pin
import time

# Define the control pins of the ultrasonic ranging module. 
Trig = Pin(13, Pin.OUT, 0) 
Echo = Pin(14, Pin.IN, 0)

distance = 0 # Define the initial distance to be 0.
soundVelocity = 340 #Set the speed of sound.

# The getDistance() function is used to drive the ultrasonic module to measure distance,
# the Trig pin keeps at high level for 10us to start the ultrasonic module.
# Echo.value() is used to read the status of ultrasonic module’s Echo pin,
# and then use timestamp function of the time module to calculate the duration of Echo
# pin’s high level,calculate the measured distance based on time and return the value.
def getDistance():
    Trig.value(1)
    time.sleep_us(10)
    Trig.value(0)
    while not Echo.value():
        pass
    pingStart = time.ticks_us()
    while Echo.value():
        pass
    pingStop = time.ticks_us()
    pingTime = time.ticks_diff(pingStop, pingStart) // 2
    distance = int(soundVelocity * pingTime // 10000)
    return distance

# Delay for 2 seconds and wait for the ultrasonic module to stabilize,
# Print data obtained from ultrasonic module every 500 milliseconds. 
time.sleep(2)
while True:
    time.sleep_ms(500)
    distance = getDistance()
    print("Distance: ", distance, "cm")
```


**6. Test Result**

Connect the wires according to the experimental wiring diagram and power on. Click ![](media/da852227207616ccd9aff28f19e02690.png)“Run current script”, the code starts executing. The "Shell" window will print the distance between the ultrasonic sensor and the object. Press“Ctrl+C”or click![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“Stop/Restart backend”to exit the program.

![](media/ce873cf513307a15f9aa58078c8dd7d6.png)

### Project 23: IR Receiver Module

![](media/80e8f8d8ddc35df9425032ec4ef783ee.png)

**1. Overview**

Infrared remote control is currently the most widely used means of communication and remote control, which has the characteristics of small volume, low power consumption, strong function and low cost. Therefore, recorder, audio equipment, air conditioning machine and toys and other small electrical devices have also used the infrared remote control.

Its transmitting circuit is the use of infrared light emitting diode to emit modulated infrared light wave. The circuit is composed of infrared receiving diode, triode or silicon photocell. They convert infrared light emitted by infrared emitter into corresponding electrical signal, and then send back amplifier.    ​    

In this experiment, we need to know how to use the infrared receiving sensor, which mainly uses the VS1838B infrared receiving sensor element. It integrates receiving, amplifying, and demodulating. The internal IC has already completed the demodulation, and the output is a digital signal. It can receive 38KHz modulated remote control signal. In the experiment, we use the IR receiver to receive the infrared signal emitted by the external infrared transmitting device, and display the received signal in the shell.

**2. Working Principle**

The main part of the IR remote control system is modulation, transmission and reception. The modulated carrier frequency is generally between 30khz and 60khz, and most of them use a square wave of 38kHz and a duty ratio of 1/3. A 4.7K pull-up resistor R3 is added to the signal end of the infrared receiver.

![](media/845973091e7fe407e7fa0e96fc1cf4f1.png)

**3. Components**

<table class="colwidths-auto docutils align-default">
<tbody>
<tr class="odd">
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/c9020c6015e55923afec197ab9d03fae.png" style="width:1.05278in;height:0.48819in" alt="4" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/6d96c844b0260ad712130945d692a7a2.jpeg" style="width:1.34444in;height:1.02986in" alt="ks0465-1" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/06218167222e41c71cdcec1c9dc08982.png" style="width:1.24444in;height:0.75069in" alt="红外接收模块" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/0d81e07a0f67700c5a396fc7e1e614e1.jpeg" style="width:0.98958in;height:0.36042in" alt="3p线" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/edbfec59fe015bd9987e4b4d542b466d.png" style="width:0.97708in;height:0.52431in" alt="USB线" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/10ccf14d80feba64bba0c1eacd02b09d.png" style="width:0.87986in;height:0.425in" alt="遥控器" /></td>
</tr>
<tr class="even">
<td>ESP32 Board*11</td>
<td>ESP32 Expansion Board*1</td>
<td><p>Keyestudio DIY</p>
<p>IR Receiver*1</p></td>
<td>3P Dupont Wire*1</td>
<td>Micro USB Cable*1</td>
<td>Remote Control*1</td>
</tr>
</tbody>
</table>

**4. Connection Diagram**

![](media/f54763e2701fefc503f275dcb9410ad0.png)

**5. Test Code**


```Python
import utime
from machine import Pin 

ird = Pin(15,Pin.IN)

act = {"1": "LLLLLLLLHHHHHHHHLHHLHLLLHLLHLHHH","2": "LLLLLLLLHHHHHHHHHLLHHLLLLHHLLHHH","3": "LLLLLLLLHHHHHHHHHLHHLLLLLHLLHHHH",
       "4": "LLLLLLLLHHHHHHHHLLHHLLLLHHLLHHHH","5": "LLLLLLLLHHHHHHHHLLLHHLLLHHHLLHHH","6": "LLLLLLLLHHHHHHHHLHHHHLHLHLLLLHLH",
       "7": "LLLLLLLLHHHHHHHHLLLHLLLLHHHLHHHH","8": "LLLLLLLLHHHHHHHHLLHHHLLLHHLLLHHH","9": "LLLLLLLLHHHHHHHHLHLHHLHLHLHLLHLH",
       "0": "LLLLLLLLHHHHHHHHLHLLHLHLHLHHLHLH","Up": "LLLLLLLLHHHHHHHHLHHLLLHLHLLHHHLH","Down": "LLLLLLLLHHHHHHHHHLHLHLLLLHLHLHHH",
       "Left": "LLLLLLLLHHHHHHHHLLHLLLHLHHLHHHLH","Right": "LLLLLLLLHHHHHHHHHHLLLLHLLLHHHHLH","Ok": "LLLLLLLLHHHHHHHHLLLLLLHLHHHHHHLH",
       "*": "LLLLLLLLHHHHHHHHLHLLLLHLHLHHHHLH","#": "LLLLLLLLHHHHHHHHLHLHLLHLHLHLHHLH"}

def read_ircode(ird):
    wait = 1
    complete = 0
    seq0 = []
    seq1 = []

    while wait == 1:
        if ird.value() == 0:
            wait = 0
    while wait == 0 and complete == 0:
        start = utime.ticks_us()
        while ird.value() == 0:
            ms1 = utime.ticks_us()
        diff = utime.ticks_diff(ms1,start)
        seq0.append(diff)
        while ird.value() == 1 and complete == 0:
            ms2 = utime.ticks_us()
            diff = utime.ticks_diff(ms2,ms1)
            if diff > 10000:
                complete = 1
        seq1.append(diff)

    code = ""
    for val in seq1:
        if val < 2000:
            if val < 700:
                code += "L"
            else:
                code += "H"
    # print(code)
    command = ""
    for k,v in act.items():
        if code == v:
            command = k
    if command == "":
        command = code
    return command

while True:
    command = read_ircode(ird)
    print(command)
    utime.sleep(0.5)
```





**6. Code Explanation**

**read\_ircode(ird) c**orresponds to the key symbol for remote control

**7. Test Result**

Connect the wires according to the experimental wiring diagram and power on. Click ![](media/da852227207616ccd9aff28f19e02690.png)“Run current script”, the code starts executing. Find the infrared remote control, pull out the insulating sheet, and press the button at the receiving head of the infrared receiving sensor. After receiving the signal, the LED on the infrared receiving sensor also starts to flash, as shown in the figure below. Press “Ctrl+C”or click![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“Stop/Restart backend”to exit the program.

![](media/ff10b0aac375db3c7ad55db88a876026.png)

### Project 24: DS1307 Clock Module

![](media/949abbbea3c8d8b36463768a39a07b51.png)

**1. Overview**

This module mainly uses the real-time clock chip DS1307, which is the I2C bus interface chip that has second, minute, hour, day, month, year and other functions as well as leap year automatic adjustment function introduced by DALLAS. It can work independently of CPU, and won‘t’ affected by the CPU main crystal oscillator and capacitance as well as keep accurate time. What‘s more, monthly cumulative error is generally less than 10 seconds.

The chip also has a clock protection circuit in case of main power failure and runs on a back-up battery that denies the CPU read and write access. At the same time, it contains automatic switching control circuit of standby power supply, so it can guarantee the accuracy of system clock in case of power failure of main power supply and other bad environment.

Going forward, the DS1307 chip internal integration has a certain capacity, with power failure protection characteristics of static RAM, which can be used to save some key data. 

In the experiment, we use the DS1307 clock module to obtain the system time and print the test results.  

**2. Working Principle**

Serial real-time clock records year, month, day, hour, minute, second and week; AM and PM indicate morning and afternoon respectively; 56 bytes of NVRAM store data; 2-wire serial port; programmable square wave output; power failure detection and automatic switching circuit; battery current is less than 500nA.

Pins description：

X1, X2：32.768kHz crystal terminal ;

VBAT: +3V input;

SDA：serial data;

SCL：serial clock;

SQW/OUT：square waves/output drivers

![](media/92b8dc82b0c2887539bd506639cfbfc0.png)

**3. Components**

<table class="colwidths-auto docutils align-default">
<tbody>
<tr class="odd">
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/c9020c6015e55923afec197ab9d03fae.png" style="width:1.05278in;height:0.48819in" alt="4" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/6d96c844b0260ad712130945d692a7a2.jpeg" style="width:1.34444in;height:1.02986in" alt="ks0465-1" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/44d6a0e867ad07a9a9733ce42a9d488a.png" style="width:1.40208in;height:0.74444in" alt="KS6072 keyestudio传感器 keyestudio 2021新款 DIY电子积木 DS1307时钟传感器模块 黑色环保 矢量图" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/269c154eda332be03643bada56070124.jpeg" style="width:0.91458in;height:0.35625in" alt="4p线" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/edbfec59fe015bd9987e4b4d542b466d.png" style="width:1.18819in;height:0.63681in" alt="USB线" /></td>
</tr>
<tr class="even">
<td>ESP32 Board*1</td>
<td>ESP32 Expansion Board*1</td>
<td>Keyestudio DS1307 Clock Module*1</td>
<td>4P Dupont Wire*1</td>
<td>Micro USB Cable*1</td>
</tr>
</tbody>
</table>

**4. Connection Diagram**

![](media/de4d2418a1b8ed0ae1c466747103a440.png)

**5. Add Library**

Open “Thonny”, click “This computer”→”D:”→”2. ESP32\_code\_MicroPython”→“lesson 36. DS1307 Real Time Clock”.
Select“<span style="color: rgb(255, 76, 65);">urtc.py</span>”，right-click and select“<span style="color: rgb(255, 76, 65);">Upload to /</span>”，waiting for the“<span style="color: rgb(255, 76, 65);">urtc.py</span>”to be uploaded to the ESP32.

![Img](./media/img-20231010131537.png)


**6. Test Code**


```Python
from machine import I2C, Pin
from urtc import DS1307 
import utime

i2c = I2C(1,scl = Pin(22),sda = Pin(21),freq = 400000)
rtc = DS1307(i2c)

year = int(input("Year : "))
month = int(input("month (Jan --> 1 , Dec --> 12): "))
date = int(input("date : "))
day = int(input("day (1 --> monday , 2 --> Tuesday ... 0 --> Sunday): "))
hour = int(input("hour (24 Hour format): "))
minute = int(input("minute : "))
second = int(input("second : "))

now = (year,month,date,day,hour,minute,second,0)
rtc.datetime(now)

#(year,month,date,day,hour,minute,second,p1) = rtc.datetime()
while True:
    DateTimeTuple = rtc.datetime()
    print(DateTimeTuple[0], end = '-')
    print(DateTimeTuple[1], end = '-')
    print(DateTimeTuple[2], end = '  ')
    print(DateTimeTuple[4], end = ':')
    print(DateTimeTuple[5], end = ':')
    print(DateTimeTuple[6], end = '  week:')
    print(DateTimeTuple[3])
    utime.sleep(1)
```




**7. Code Explanation**

**rtc.datetime()：** Return a tuple of time. When the program is running, we set the "please input" program, run the code, it will prompt us to input the time and date, after the input is completed, the data will be printed every second.

**DateTimeTuple\[0\]:** save years

**DateTimeTuple\[1\]:** save months

**DateTimeTuple\[2\]**: save days

**DateTimeTuple\[3\]**: save weeks

**Rtc.GetDateTime().Month():** return months

**DateTimeTuple\[4\]:** save hours

**DateTimeTuple\[5\]**: save minutes

**DateTimeTuple\[6\]:** save seconds

**8. Test Result**

Connect the wires according to the experimental wiring diagram and power on. Click ![](media/da852227207616ccd9aff28f19e02690.png)“Run current script”, the code starts executing. Then the shell will display “Year：”. Then we enter year, month, day, hour, minute and second, once complete, printed the data every second, as shown below. Press “Ctrl+C”or click ![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“Stop/Restart backend”to exit the program.

![](media/db5ed7d9d70655d0d4347aed286c76dd.png)

### Project 25: TM1650 4-Digit Tube Display

![](media/f698ea56391906278b7c8064fca42bb3.jpeg)

**1. Overview**

This module is mainly composed of a 0.36 inch red common cathode 4-digit digital tube, and its driver chip is TM1650. When using it, we only need two signal lines to make the single-chip microcomputer control a 4-bit digit tube, which greatly saves the IO port resources of the control board.

TM1650 is a special circuit for LED (light emitting diode display) drive control. It integrates MCU input and output control digital interface, data latch, LED drivers, keyboard scanning, brightness adjustment and other circuits.

TM1650 has stable performance, reliable quality and strong anti-interference ability.

It can be applied to the application of long-term continuous working for 24 hours.

TM1650 uses 2-wire serial transmission protocol for communication (note that this data transmission protocol is not a standard I2C protocol). The chip can drive the digital tube and save MCU pin resources through two pins and MCU communication.

**2. Working Principle**

TM1650 adopts IIC treaty, which uses DIO and CLK buses.

![](media/c7b895791863dfc2663800ce90f61c89.png)

**Data command setting**: 0x48 means that we light up the digital tube, instead of enable the function of key scanning

![](media/09585b52bed3d4112d59a611c3c3f262.png)

**Command display setting:**

bit\[6:4\]：set the brightness of tube display, and 000 is brightest

bit\[3\]：set to show decimal points

bit\[0\]：start the display of the tube display

**3. Components**

<table class="colwidths-auto docutils align-default">
<tbody>
<tr class="odd">
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/c9020c6015e55923afec197ab9d03fae.png" style="width:1.05278in;height:0.48819in" alt="4" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/6d96c844b0260ad712130945d692a7a2.jpeg" style="width:1.34444in;height:1.02986in" alt="ks0465-1" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/f47b077303226cce504ea7734826dfc9.png" style="width:0.94514in;height:0.52569in" alt="四位数码管模块" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/269c154eda332be03643bada56070124.jpeg" style="width:0.91458in;height:0.35625in" alt="4p线" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/edbfec59fe015bd9987e4b4d542b466d.png" style="width:1.18819in;height:0.63681in" alt="USB线" /></td>
</tr>
<tr class="even">
<td>ESP32 Board*1</td>
<td>ESP32 Expansion Board*1</td>
<td>Keyestudio TM16504-Digit Segment Display*1</td>
<td>4P Dupont Wire*1</td>
<td>Micro USB Cable*1</td>
</tr>
</tbody>
</table>

**4. Connection Diagram**

![](media/08a0d34d55b5e4215c77fbf8f656c9a9.png)

**5. Test Code**


```Python
from machine import Pin
import time

# definitions for TM1650
ADDR_DIS = 0x48  #mode command
ADDR_KEY = 0x49  #read key value command

# definitions for brightness
BRIGHT_DARKEST = 0
BRIGHT_TYPICAL = 2
BRIGHTEST      = 7

on  = 1
off = 0

# number:0~9
NUM = [0x3f,0x06,0x5b,0x4f,0x66,0x6d,0x7d,0x07,0x7f,0x6f] 
# DIG = [0x68,0x6a,0x6c,0x6e]
DIG = [0x6e,0x6c,0x6a,0x68]
DOT = [0,0,0,0]

clkPin = 22
dioPin = 21
clk = Pin(clkPin, Pin.OUT)
dio = Pin(dioPin, Pin.OUT)

DisplayCommand = 0

def writeByte(wr_data):
    global clk,dio
    for i in range(8):
        if(wr_data & 0x80 == 0x80):
            dio.value(1)
        else:
            dio.value(0)
        clk.value(0)
        time.sleep(0.0001)
        clk.value(1)
        time.sleep(0.0001)
        clk.value(0)
        wr_data <<= 1
    return

def start():
    global clk,dio
    dio.value(1)
    clk.value(1)
    time.sleep(0.0001)
    dio.value(0)
    return
    
def ack():
    global clk,dio
    dy = 0
    clk.value(0)
    time.sleep(0.0001)
    dio = Pin(dioPin, Pin.IN)
    while(dio.value() == 1):
        time.sleep(0.0001)
        dy += 1
        if(dy>5000):
            break
    clk.value(1)
    time.sleep(0.0001)
    clk.value(0)
    dio = Pin(dioPin, Pin.OUT)
    return 
    
def stop():
    global clk,dio
    dio.value(0)
    clk.value(1)
    time.sleep(0.0001)
    dio.value(1)
    return
    
def displayBit(bit, num):
    global ADDR_DIS
    if(num > 9 and bit > 4):
        return
    start()
    writeByte(ADDR_DIS)
    ack()
    writeByte(DisplayCommand)
    ack()
    stop()
    start()
    writeByte(DIG[bit-1])
    ack()
    if(DOT[bit-1] == 1):
        writeByte(NUM[num] | 0x80)
    else:
        writeByte(NUM[num])
    ack()
    stop()
    return
    
def clearBit(bit):
    if(bit > 4):
        return
    start()
    writeByte(ADDR_DIS)
    ack()
    writeByte(DisplayCommand)
    ack()
    stop()
    start()
    writeByte(DIG[bit-1])
    ack()
    writeByte(0x00)
    ack()
    stop()
    return
    
    
def setBrightness(b = BRIGHT_TYPICAL):
    global DisplayCommand,brightness
    DisplayCommand = (DisplayCommand & 0x0f)+(b<<4)
    return

def setMode(segment = 0):
    global DisplayCommand
    DisplayCommand = (DisplayCommand & 0xf7)+(segment<<3)
    return
    
def displayOnOFF(OnOff = 1):
    global DisplayCommand
    DisplayCommand = (DisplayCommand & 0xfe)+OnOff
    return

def displayDot(bit, OnOff):
    if(bit > 4):
        return
    if(OnOff == 1): 
        DOT[bit-1] = 1;
    else:
        DOT[bit-1] = 0;
    return
        
def InitDigitalTube():
    setBrightness(2)
    setMode(0)
    displayOnOFF(1)
    for _ in range(4):
        clearBit(_)
    return

def ShowNum(num): #0~9999
    displayBit(1,num%10)
    if(num < 10):
        clearBit(2)
        clearBit(3)
        clearBit(4)
    if(num > 9 and num < 100):
        displayBit(2,num//10%10)
        clearBit(3)
        clearBit(4)
    if(num > 99 and num < 1000):
        displayBit(2,num//10%10)
        displayBit(3,num//100%10)
        clearBit(4)
    if(num > 999 and num < 10000):
        displayBit(2,num//10%10)
        displayBit(3,num//100%10)
        displayBit(4,num//1000)

InitDigitalTube()

while True:
    #displayDot(1,on)     # on or off, DigitalTube.Display(bit,number); bit=1---4  number=0---9
    for i in range(0,9999):
        ShowNum(i)
        time.sleep(0.01)
```




**6. Code Explanation**

**clkPin = 22、dioPin = 21is pin number**，CLK is connected to GPIO22，DIO is connected to GPIO21. We can set any two pins at random.

**displayBit(bit, num):** show numbers at bit(1\~4) bit num(0\~9)

**clearBit(bit): clear up** bit(1\~4)

**setBrightness():** brightness setting

**displayOnOFF():** 0 means OFF, 1 means ON

**displayDot(bit, OnOff):** shows dots，0 means OFF, 1 means ON

**ShowNum(num):** show integer num，in the range of 0\~9999

**7. Test Result**

Connect the wires according to the experimental wiring diagram and power on. Click ![](media/da852227207616ccd9aff28f19e02690.png)“Run current script”, the code starts executing. The 4-digit tube display will show integer from 0 to 99999, an increase of 1 for each 10ms, then start from 0 once reaching 99999. Press “Ctrl+C”or click ![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“Stop/Restart backend”to exit the program.

### Project 26: HT16K33\_8X8 Dot Matrix Module

![](media/431b6c4abd63b99219658a03d24de991.jpeg)

**1. Overview**

What is the dot matrix display?

If we apply the previous circuit, there will be must one IO port to control only one LED. When more LED need to be controlled, we may adopt a dot matrix.
The 8X8 dot matrix is composed of 64 light-emitting diodes, and each light-emitting diode is placed at the intersection of the row line and the column line. 
Refer to the experimental schematic diagram below, when the corresponding column is set to a high level and a certain row to low, the corresponding diode will light up. For instance, set pin 13 to a high level and pin 9 to low, and then the first LED will light up.
In the experiment, we display icons via this dot matrix.

**2. Working Principle**

As the schematic diagram shown, to light up the LED at the first row and column, we only need to set C1 to high level and R1 to low level. To turn on LEDs at the first row, we set R1 to low level and C1-C8 to high level.

16 IO ports are needed, which will highly waste the MCU resources.

Therefore, we designed this module, using the HT16K33 chip to drive an 8\*8 dot matrix, which greatly saves the resources of the single-chip microcomputer.

There are three DIP switches on the module, all of which are set to I2C communication address. The setting method is shown below. A0，A1 and A2 are grounded, that is, the address is 0x70.

![Img](./media/img-20231010134119.png)

**3. Components**

<table class="colwidths-auto docutils align-default">
<tbody>
<tr class="odd">
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/c9020c6015e55923afec197ab9d03fae.png" style="width:1.05278in;height:0.48819in" alt="4" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/6d96c844b0260ad712130945d692a7a2.jpeg" style="width:1.34444in;height:1.02986in" alt="ks0465-1" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/713307c9cb50d067a014dee9522afe15.png" style="width:0.99722in;height:0.49861in" alt="_8X8点阵模块" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/269c154eda332be03643bada56070124.jpeg" style="width:0.91458in;height:0.35625in" alt="4p线" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/edbfec59fe015bd9987e4b4d542b466d.png" style="width:1.18819in;height:0.63681in" alt="USB线" /></td>
</tr>
<tr class="even">
<td>ESP32 Board*1</td>
<td>ESP32 Expansion Board*1</td>
<td><p>Keyestudio HT16K33_</p>
<p>8X8 Dot Matrix*1</p></td>
<td>4P Dupont Wire*1</td>
<td>Micro USB Cable*1</td>
</tr>
</tbody>
</table>

**4. Connection Diagram**

![](media/d3f2f2968ff861d04e909cf330986652.png)

**5. Add Library**

Open“Thonny”, click“This computer”→“D:”→“2. ESP32\_code\_MicroPython”→“lesson 38. HT16K33 dot matrix”.
Select“<span style="color: rgb(255, 76, 65);">ht16k33.py</span>”and“<span style="color: rgb(255, 76, 65);">ht16k33matrix.py</span>”，right-click and select“<span style="color: rgb(255, 76, 65);">Upload to /</span>”，waiting for the “<span style="color: rgb(255, 76, 65);">ht16k33.py</span>”and“<span style="color: rgb(255, 76, 65);">ht16k33matrix.py</span>”to be uploaded to the ESP32.

![Img](./media/img-20231010132031.png)
![Img](./media/img-20231010132036.png)


**6. Test Code**


```Python
# IMPORTS
import utime as time
from machine import I2C, Pin, RTC
from ht16k33matrix import HT16K33Matrix

# CONSTANTS
DELAY = 0.01
PAUSE = 3

# START
if __name__ == '__main__':
    i2c = I2C(scl=Pin(22), sda=Pin(21))
    display = HT16K33Matrix(i2c)
    display.set_brightness(2)

    # Draw a custom icon on the LED
    icon = b"\x00\x66\x00\x00\x18\x42\x3c\x00"
    display.set_icon(icon).draw()
    # Rotate the icon
    display.set_angle(0).draw()
    time.sleep(PAUSE)
```






**7. Test Result**

Connect the wires according to the experimental wiring diagram and power on. Click ![](media/da852227207616ccd9aff28f19e02690.png)“Run current script”, the code starts executing. The dot matrix displays a“ smile ”pattern. Press “Ctrl+C”or click ![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“Stop/Restart backend”to exit the program.

## 3. Comprehensive Experiments

The previous projects are related to single sensor or module. In the following part, we will combine various sensors and modules to create some comprehensive experiments to perform special functions.

### Project 27: Button-controlled LED

![](media/50740b22d16151d490b8494b0bff4f6e.jpeg)

**1. Overview**

In this lesson, we will make an extension experiment with a button and an LED. When the button is pressed and low levels are output, the LED will light up; when the button is released, the LED will go off. Then we can control a module with another module.

**2. Components**

<table class="colwidths-auto docutils align-default">
<tbody>
<tr class="odd">
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/c9020c6015e55923afec197ab9d03fae.png" style="width:1.05278in;height:0.48819in" alt="4" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/6d96c844b0260ad712130945d692a7a2.jpeg" style="width:1.07222in;height:0.82083in" alt="ks0465-1" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/f0ef7a5a2e7eebb09e91f73cb2a6caf3.png" style="width:1.06944in;height:0.75972in" alt="白色LED模块" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/1aafa8910f5184973f1c913c19489fbd.png" style="width:1.07292in;height:0.76389in" alt="单路按键模块" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/0d81e07a0f67700c5a396fc7e1e614e1.jpeg" style="width:0.98958in;height:0.36042in" alt="3p线" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/edbfec59fe015bd9987e4b4d542b466d.png" style="width:1.18819in;height:0.63681in" alt="USB线" /></td>
</tr>
<tr class="even">
<td>ESP32 Board*1</td>
<td>ESP32 Expansion Board*1</td>
<td>Keyestudio White LED Module*1</td>
<td>Keyestudio DIY Button Module*1</td>
<td>3P Dupont Wire*2</td>
<td>Micro USB Cable*1</td>
</tr>
</tbody>
</table>

**3. Connection Diagram**

![](media/378de9cb95275a6a1dec9adbf2f15eaa.png)

**4. Test Code**

```Python
from machine import Pin
import time

led = Pin(4, Pin.OUT) # create LED object from Pin 4,Set Pin 4 to output                   
button = Pin(15, Pin.IN, Pin.PULL_UP) #Create button object from Pin15,Set GP15 to input

#Customize a function and name it reverseGPIO(),which reverses the output level of the LED
def reverseGPIO():
    if led.value():
        led.value(0)     #Set led turn off
    else:
        led.value(1)     #Set led turn on

try:
    while True:
        if not button.value():
            time.sleep_ms(20)
            if not button.value():
                reverseGPIO()
                while not button.value():
                    time.sleep_ms(20)
except:
    pass
```



**5. Test Result**

Connect the wires according to the experimental wiring diagram and power on. Click ![](media/da852227207616ccd9aff28f19e02690.png)“Run current script”, the code starts executing. When the button is pressed, the LED will light up, when pressed again, the LED will go off, cycle this operation. Press “Ctrl+C”or “Stop/Restart backend”to exit the program.

### Project 28: Alarm Experiment

![](media/6db3cb7d3a91e700a3b651c1f0edb7a5.jpeg)

**1. Overview**

In the previous experiment, we control an output module though an input module. In this lesson, we will make an experiment that the active buzzer will emit sounds once an obstacle appears.

**2. Components**

<table class="colwidths-auto docutils align-default">
<tbody>
<tr class="odd">
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/c9020c6015e55923afec197ab9d03fae.png" style="width:1.65278in;height:0.48819in" alt="4" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/6d96c844b0260ad712130945d692a7a2.jpeg" style="width:1.05556in;height:0.80833in" alt="ks0465-1" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/ac83d2c470cd6c345f17feed3bce5358.png" style="width:1.05903in;height:0.70556in" alt="避障传感器" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/cbc890daba907eee365bdaacf1f509a8.png" style="width:1.03056in;height:0.70764in" alt="有源蜂鸣器模块" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/0d81e07a0f67700c5a396fc7e1e614e1.jpeg" style="width:0.98958in;height:0.36042in" alt="3p线" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/edbfec59fe015bd9987e4b4d542b466d.png" style="width:1.08819in;height:0.45208in" alt="USB线" /></td>
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

### Project 29: Intrusion Detection

![](media/b7828b9e5ee615a151567e20d35db90f.png)

**1. Description**

In this experiment, we use a PIR motion sensor to control an active buzzer to emit sounds and the onboard LED to flash rapidly.

**2. Required Components**

<table class="colwidths-auto docutils align-default">
<tbody>
<tr class="odd">
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/c9020c6015e55923afec197ab9d03fae.png" style="width:1.05278in;height:0.48819in" alt="4" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/6d96c844b0260ad712130945d692a7a2.jpeg" style="width:1.34444in;height:1.02986in" alt="ks0465-1" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/256a8301b740dfb2981a635a4b575ba0.png" style="width:1.07361in;height:0.76458in" alt="人体红外热释传感器" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/cbc890daba907eee365bdaacf1f509a8.png" style="width:1.09028in;height:0.7875in" alt="有源蜂鸣器模块" /></td>
</tr>
<tr class="even">
<td>ESP32 Board*1</td>
<td>ESP32 Expansion Board*1</td>
<td>Keyestudio DIY PIR Motion Sensor*1</td>
<td>Keyestudio DIY Active Buzzer*1</td>
</tr>
<tr class="odd">
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/12ecb079cf6481a6f0f04d6b7bb31fd8.png" style="width:1.00417in;height:0.73889in" alt="白色LED模块" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/0d81e07a0f67700c5a396fc7e1e614e1.jpeg" style="width:0.98958in;height:0.36042in" alt="3p线" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/edbfec59fe015bd9987e4b4d542b466d.png" style="width:0.89722in;height:0.37292in" alt="USB线" /></td>
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

### Project 30: Rotary Encoder control RGB

![](media/c6b4f1cedef06ed68d1c2e5ccf5c17d2.jpeg)

**1. Introduction**

In this lesson, we will control the LED on the RGB module to show different colors through a rotary encoder.

When designing the code, we need to divide the obtained values by 3 to get the remainders. The remainder is 0 and the LED will become red. The remainder is 1, the LED will become green. The remainder is 2, the LED will turn blue.

**2. Components**

<table class="colwidths-auto docutils align-default">
<tbody>
<tr class="odd">
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/c9020c6015e55923afec197ab9d03fae.png" style="width:1.05278in;height:0.48819in" alt="4" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/6d96c844b0260ad712130945d692a7a2.jpeg" style="width:1.34444in;height:1.02986in" alt="ks0465-1" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/eb9d1b363af72bc105ce38cb9e4d99b1.png" style="width:1.03472in;height:0.78125in" alt="共阴RGB模块" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/989ee8ccd2a016dcaeb0bef68d55e912.png" style="width:1.17708in;height:0.73264in" alt="旋转编码器模块" /></td>
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
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/fc3fd9c0110b04d1af77a2ff8c01a10a.png" style="width:1.36736in;height:0.57361in" alt="5p线" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/269c154eda332be03643bada56070124.jpeg" style="width:1.46875in;height:0.57222in" alt="4p线" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/edbfec59fe015bd9987e4b4d542b466d.png" style="width:0.89722in;height:0.37292in" alt="USB线" /></td>
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

![Img](./media/img-20231010134724.png)
![Img](./media/img-20231010134730.png)


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

### Project 31: Rotary Potentiometer

![](media/f71165ab140ae6b2aac093dc75785c96.jpeg)

**1. Introduction**

In the previous courses, we did experiments of breathing light and controlling LED with button. In this course, we do these two experiments by controlling the brightness of LED through an adjustable potentiometer. The brightness of LED is controlled by PWM values, and the range of analog values is 0 to 4095 and the PWM value range is 0-255.

After the code is set successfully, we can control the brightness of the LED on the module by rotating the potentiometer.

**2. Required Components**

<table class="colwidths-auto docutils align-default">
<tbody>
<tr class="odd">
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/c9020c6015e55923afec197ab9d03fae.png" style="width:1.55278in;height:0.48819in" alt="4" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/6d96c844b0260ad712130945d692a7a2.jpeg" style="width:1.01528in;height:0.77708in" alt="ks0465-1" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/f0ef7a5a2e7eebb09e91f73cb2a6caf3.png" style="width:1.0375in;height:0.74931in" alt="白色LED模块" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/a0eebfcd8f84c3fbac526e9910e66692.png" style="width:1.11667in;height:0.82292in" alt="旋转电位器传感器" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/0d81e07a0f67700c5a396fc7e1e614e1.jpeg" style="width:0.98958in;height:0.36042in" alt="3p线" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/edbfec59fe015bd9987e4b4d542b466d.png" style="width:1.18819in;height:0.63681in" alt="USB线" /></td>
</tr>
<tr class="even">
<td>ESP32 Board*1</td>
<td>ESP32 Expansion Board*1</td>
<td>Keyestudio White LED*1</td>
<td>Keyestudio Rotary Potentiometer*1</td>
<td>3P Dupont Wire*2</td>
<td>Micro USB Cable*1</td>
</tr>
</tbody>
</table>

**3. Connection Diagram**

![](media/7f24723673e622d23fbe0a3cdbd21d69.png)

**4. Test Code**


```Python
from machine import Pin,PWM,ADC
import time

pwm =PWM(Pin(15,Pin.OUT),1000)
adc=ADC(Pin(34))
adc.atten(ADC.ATTN_11DB)
adc.width(ADC.WIDTH_10BIT)

try:
    while True:
        adcValue=adc.read()
        pwm.duty(adcValue)
        print(adc.read())
        time.sleep_ms(100)
except:
    pwm.deinit()
```


**5. Code Explanation**

It is easy to control the brightness of the LED light by a potentiometer. Here we can find that MicroPython unifies the value range
of the ADC between 0 and 1023, and assigns values directly, which is simple and convenient.

**6. Test Result**

Connect the wires according to the experimental wiring diagram and power on. Click ![](media/da852227207616ccd9aff28f19e02690.png)“Run current script”, the code starts executing. Rotating the potentiometer on the module can adjust the brightness of the LED on the LED module. Press “Ctrl+C”or click![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“Stop/Restart backend”to exit the program.


### Project 32: Sound Activated Light

![](media/f3ddb58e83a92a888d3e1d66f7456170.png)

**1. Introduction**

In this lesson, we will make a smart sound activated light using a sound sensor and an LED module. When we make a sound, the light will automatically turn on; when there is no sound, the lights will automatically turn off. How it works? Because the sound-controlled light is equipped with a sound sensor, and this sensor converts the intensity of external sound into a corresponding value. Then set a threshold, when the threshold is exceeded, the light will turn on, and when it is not exceeded, the light will go out.

**2. Components**

<table class="colwidths-auto docutils align-default">
<tbody>
<tr class="odd">
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/c9020c6015e55923afec197ab9d03fae.png" style="width:0.925in;height:0.42917in" alt="4" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/6d96c844b0260ad712130945d692a7a2.jpeg" style="width:0.97569in;height:0.74792in" alt="ks0465-1" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/cf7b54ba090f4e34025101cf9ece26d1.png" style="width:1.00903in;height:0.7125in" alt="声音传感器" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/f0ef7a5a2e7eebb09e91f73cb2a6caf3.png" style="width:1.02153in;height:0.72847in" alt="白色LED模块" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/0d81e07a0f67700c5a396fc7e1e614e1.jpeg" style="width:0.98958in;height:0.36042in" alt="3p线" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/edbfec59fe015bd9987e4b4d542b466d.png" style="width:0.94583in;height:0.44375in" alt="USB线" /></td>
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

### Project 33: Ultrasonic Radar

![](media/19a7c30e24f0ec39da94912c5535b791.png)

**1. Description**

![](media/38037219a4908755dbedc422be1ab61b.jpeg)

We know that bats use echoes to determine the direction and the location of their preys. In real life, sonar is used to detect sounds in the water. Since the attenuation rate of electromagnetic waves in water is very high, it cannot be used to detect signals, however, the attenuation rate of sound waves in the water is much smaller, so sound waves are most commonly used underwater for observation and measurement. In this experiment, we will use a speaker module, an RGB module and a 4-digit tube display to make a device for detection through ultrasonic.

**2. Required Components**

<table class="colwidths-auto docutils align-default">
<tbody>
<tr class="odd">
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/c9020c6015e55923afec197ab9d03fae.png" style="width:1.05278in;height:0.48819in" alt="4" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/6d96c844b0260ad712130945d692a7a2.jpeg" style="width:1.09028in;height:0.83542in" alt="ks0465-1" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/4a358f0f161b2e4dcae43f9315902ef3.png" style="width:1.02986in;height:0.56806in" alt="超声波模块" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/1ef2dd7f7fd91d208e726ef074a02dca.png" style="width:1.32986in;height:0.71667in" alt="8002b功放 喇叭模块" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/eb9d1b363af72bc105ce38cb9e4d99b1.png" style="width:1.03542in;height:0.68264in" alt="共阴RGB模块" /></td>
</tr>
<tr class="even">
<td>ESP32 Board*1</td>
<td>ESP32 Expansion Board*1</td>
<td>Keyestudio HC-SR04 Ultrasonic Sensor*1</td>
<td>Keyestudio 8002b Power Amplifier*1</td>
<td>Keyestudio DIY Common Cathode RGB Module *1</td>
</tr>
<tr class="odd">
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/8f646a7dfa38852a8eccb5e85eb7341a.png" style="width:1.02917in;height:0.57222in" alt="四位数码管模块" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/269c154eda332be03643bada56070124.jpeg" style="width:1.02292in;height:0.39861in" alt="4p线" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/0d81e07a0f67700c5a396fc7e1e614e1.jpeg" style="width:0.98958in;height:0.36042in" alt="3p线" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/edbfec59fe015bd9987e4b4d542b466d.png" style="width:0.94583in;height:0.44375in" alt="USB线" /></td>
<td></td>
</tr>
<tr class="even">
<td>Keyestudio DIY TM1650 4-Digit Display*1</td>
<td>4P Dupont Wire*3</td>
<td>3P Dupont Wire*1</td>
<td>Micro USB Cable*1</td>
<td></td>
</tr>
</tbody>
</table>

**3. Connection Diagram**

![](media/3d6e86b75df96354e05447244d2fee68.png)

**4. Test Code**


```Python
from machine import Pin, PWM
import utime
 
# definitions for TM1650
ADDR_DIS = 0x48  #mode command
ADDR_KEY = 0x49  #read key value command

# definitions for brightness
BRIGHT_DARKEST = 0
BRIGHT_TYPICAL = 2
BRIGHTEST      = 7

on  = 1
off = 0

# number:0~9
NUM = [0x3f,0x06,0x5b,0x4f,0x66,0x6d,0x7d,0x07,0x7f,0x6f] 
# DIG = [0x68,0x6a,0x6c,0x6e]
DIG = [0x6e,0x6c,0x6a,0x68]
DOT = [0,0,0,0]

clkPin = 22
dioPin = 21
clk = Pin(clkPin, Pin.OUT)
dio = Pin(dioPin, Pin.OUT)

DisplayCommand = 0

def writeByte(wr_data):
    global clk,dio
    for i in range(8):
        if(wr_data & 0x80 == 0x80):
            dio.value(1)
        else:
            dio.value(0)
        clk.value(0)
        utime.sleep(0.0001)
        clk.value(1)
        utime.sleep(0.0001)
        clk.value(0)
        wr_data <<= 1
    return

def start():
    global clk,dio
    dio.value(1)
    clk.value(1)
    utime.sleep(0.0001)
    dio.value(0)
    return
    
def ack():
    global clk,dio
    dy = 0
    clk.value(0)
    utime.sleep(0.0001)
    dio = Pin(dioPin, Pin.IN)
    while(dio.value() == 1):
        utime.sleep(0.0001)
        dy += 1
        if(dy>5000):
            break
    clk.value(1)
    utime.sleep(0.0001)
    clk.value(0)
    dio = Pin(dioPin, Pin.OUT)
    return
    
def stop():
    global clk,dio
    dio.value(0)
    clk.value(1)
    utime.sleep(0.0001)
    dio.value(1)
    return
    
def displayBit(bit, num):
    global ADDR_DIS
    if(num > 9 and bit > 4):
        return
    start()
    writeByte(ADDR_DIS)
    ack()
    writeByte(DisplayCommand)
    ack()
    stop()
    start()
    writeByte(DIG[bit-1])
    ack()
    if(DOT[bit-1] == 1):
        writeByte(NUM[num] | 0x80)
    else:
        writeByte(NUM[num])
    ack()
    stop()
    return
    
def clearBit(bit):
    if(bit > 4):
        return
    start()
    writeByte(ADDR_DIS)
    ack()
    writeByte(DisplayCommand)
    ack()
    stop()
    start()
    writeByte(DIG[bit-1])
    ack()
    writeByte(0x00)
    ack()
    stop()
    return
    
    
def setBrightness(b = BRIGHT_TYPICAL):
    global DisplayCommand,brightness
    DisplayCommand = (DisplayCommand & 0x0f)+(b<<4)
    return

def setMode(segment = 0):
    global DisplayCommand
    DisplayCommand = (DisplayCommand & 0xf7)+(segment<<3)
    return
    
def displayOnOFF(OnOff = 1):
    global DisplayCommand
    DisplayCommand = (DisplayCommand & 0xfe)+OnOff
    return

def displayDot(bit, OnOff):
    if(bit > 4):
        return
    if(OnOff == 1): 
        DOT[bit-1] = 1;
    else:
        DOT[bit-1] = 0;
    return
        
def InitDigitalTube():
    setBrightness(2)
    setMode(0)
    displayOnOFF(1)
    for _ in range(4):
        clearBit(_)
    return

def ShowNum(num): #0~9999
    displayBit(1,num%10)
    if(num < 10):
        clearBit(2)
        clearBit(3)
        clearBit(4)
    if(num > 9 and num < 100):
        displayBit(2,num//10%10)
        clearBit(3)
        clearBit(4)
    if(num > 99 and num < 1000):
        displayBit(2,num//10%10)
        displayBit(3,num//100%10)
        clearBit(4)
    if(num > 999 and num < 10000):
        displayBit(2,num//10%10)
        displayBit(3,num//100%10)
        displayBit(4,num//1000)

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

# Ultrasonic ranging, unit: cm
def getDistance(trigger, echo):
    # Generates a 10us square wave
    trigger.value(0)   #A short low level is given beforehand to ensure a clean high pulse:
    utime.sleep_us(2)
    trigger.value(1)
    utime.sleep_us(10)#After pulling high, wait 10 microseconds and immediately set it to low
    trigger.value(0)
    
    while echo.value() == 0: #Establish a while loop to detect whether the echo pin value is 0 and record the time at that time
        start = utime.ticks_us()
    while echo.value() == 1: #Establish a while loop to check whether the echo pin value is 1 and record the time at that time
        end = utime.ticks_us()
    d = (end - start) * 0.0343 / 2 #The travel time of the sound wave x the speed of sound (343.2 m/s, 0.0343 cm/microsecond), and the distance back and forth divided by 2.
    return d

# set the pin
trigger = Pin(13, Pin.OUT)
echo = Pin(14, Pin.IN)

buzzer = PWM(Pin(18))
def playtone(frequency):
    buzzer.duty(1000)
    buzzer.freq(frequency)

def bequiet():
    buzzer.duty(0)
    
# main program
InitDigitalTube()
while True:
    distance = int(getDistance(trigger, echo))
    ShowNum(distance)
    if distance <= 10:
        playtone(880)
        utime.sleep(0.1)
        bequiet()
        light(1023, 0, 0)
    elif distance <= 20:
        playtone(532)
        utime.sleep(0.2)
        bequiet()
        light(0, 0, 1023)
    else:
        light(0, 1023, 0)
```

**5. Code Explanation**

We set sound frequency and light color by adjusting different distance range.

We can adjust the distance range in the code.

**6. Test Result**

Connect the wires according to the experimental wiring diagram and power on. Click ![](media/da852227207616ccd9aff28f19e02690.png)“Run current script”, the code starts executing. When the ultrasonic sensor detects different distances(within 20 cm), the buzzer will produce different frequencies of sound, the RGB will show different colors, and the measured distances are displayed on the 4-digit tube display. Press “Ctrl+C”or click ![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“Stop/Restart backend”to exit the program.

### Project 34: IR Remote Control

![](media/6e823de7db355fde0bc5fcb7c1cdc705.jpeg)

**1. Introduction**

In the previous experiments, we learned how to turn on/off the LED and adjust its brightness via PWM and print the button value of the IR  remote control in the Shell window. Herein, we use an infrared remote control to turn on/off an LED.

**2. Components**

<table class="colwidths-auto docutils align-default">
<tbody>
<tr class="odd">
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/c9020c6015e55923afec197ab9d03fae.png" style="width:1.05278in;height:0.48819in" alt="4" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/6d96c844b0260ad712130945d692a7a2.jpeg" style="width:1.34444in;height:1.02986in" alt="ks0465-1" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/f0ef7a5a2e7eebb09e91f73cb2a6caf3.png" style="width:1.17292in;height:0.79792in" alt="白色LED模块" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/6d2903250f8e18898973c545ca497393.png" style="width:1.17639in;height:0.79375in" alt="红外接收模块" /></td>
</tr>
<tr class="even">
<td>ESP32 Board*1</td>
<td>ESP32 Expansion Board*1</td>
<td>Keyestudio White LED Module*1</td>
<td>Keyestudio DIY IR Receiver*1</td>
</tr>
<tr class="odd">
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/edbfec59fe015bd9987e4b4d542b466d.png" style="width:0.94583in;height:0.44375in" alt="USB线" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/10ccf14d80feba64bba0c1eacd02b09d.png" style="width:1.3in;height:0.62847in" alt="遥控器" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/0d81e07a0f67700c5a396fc7e1e614e1.jpeg" style="width:0.98958in;height:0.36042in" alt="3p线" /></td>
<td></td>
</tr>
<tr class="even">
<td>Micro USB Cable*1</td>
<td>IR Remote Control*1</td>
<td>3P Dupont Wire*2</td>
<td></td>
</tr>
</tbody>
</table>

**3. Connection Diagram**

![](media/e00f371661e0fa08c98e84d3d22a110c.png)

**4. Test Code**


```Python
import time
from machine import Pin

led = Pin(4, Pin.OUT)
ird = Pin(15,Pin.IN)

act = {"1": "LLLLLLLLHHHHHHHHLHHLHLLLHLLHLHHH","2": "LLLLLLLLHHHHHHHHHLLHHLLLLHHLLHHH","3": "LLLLLLLLHHHHHHHHHLHHLLLLLHLLHHHH",
       "4": "LLLLLLLLHHHHHHHHLLHHLLLLHHLLHHHH","5": "LLLLLLLLHHHHHHHHLLLHHLLLHHHLLHHH","6": "LLLLLLLLHHHHHHHHLHHHHLHLHLLLLHLH",
       "7": "LLLLLLLLHHHHHHHHLLLHLLLLHHHLHHHH","8": "LLLLLLLLHHHHHHHHLLHHHLLLHHLLLHHH","9": "LLLLLLLLHHHHHHHHLHLHHLHLHLHLLHLH",
       "0": "LLLLLLLLHHHHHHHHLHLLHLHLHLHHLHLH","Up": "LLLLLLLLHHHHHHHHLHHLLLHLHLLHHHLH","Down": "LLLLLLLLHHHHHHHHHLHLHLLLLHLHLHHH",
       "Left": "LLLLLLLLHHHHHHHHLLHLLLHLHHLHHHLH","Right": "LLLLLLLLHHHHHHHHHHLLLLHLLLHHHHLH","Ok": "LLLLLLLLHHHHHHHHLLLLLLHLHHHHHHLH",
       "*": "LLLLLLLLHHHHHHHHLHLLLLHLHLHHHHLH","#": "LLLLLLLLHHHHHHHHLHLHLLHLHLHLHHLH"}

def read_ircode(ird):
    wait = 1
    complete = 0
    seq0 = []
    seq1 = []

    while wait == 1:
        if ird.value() == 0:
            wait = 0
    while wait == 0 and complete == 0:
        start = time.ticks_us()
        while ird.value() == 0:
            ms1 = time.ticks_us()
        diff = time.ticks_diff(ms1,start)
        seq0.append(diff)
        while ird.value() == 1 and complete == 0:
            ms2 = time.ticks_us()
            diff = time.ticks_diff(ms2,ms1)
            if diff > 10000:
                complete = 1
        seq1.append(diff)

    code = ""
    for val in seq1:
        if val < 2000:
            if val < 700:
                code += "L"
            else:
                code += "H"
    # print(code)
    command = ""
    for k,v in act.items():
        if code == v:
            command = k
    if command == "":
        command = code
    return command

flag = False
while True:
#     global flag
    command = read_ircode(ird)
    print(command, end = "  ")
    print(flag, end = "  ")
    if command == "Ok":
        if flag == True:
            led.value(1)
            flag = False
            print("led on")
        else:
            led.value(0)
            flag = True
            print("led off")
    time.sleep(0.1)
```

**5. Code Explanation**

We define a boolean variable. There are two boolean variables. true(true) or false (false).

When we press the OK button, the value of infrared reception is OK. At this time, we need to set a boolean variable flag. When the flag is true(true), the LED is turned on, and when it is false (false), the LED is turned off and turned on. After the LED is on and set it to false. We press the OK key, the LED will be off.

**6. Test Result**

Connect the wires according to the experimental wiring diagram and power on. Click ![](media/da852227207616ccd9aff28f19e02690.png)“Run current script”, the code starts executing. Press the OK button of the remote, the LED will be on, press it again, the LED will be off.

Press “Ctrl+C”or click ![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“Stop/Restart backend”to exit the program.

![](media/ad0be693b3f956103a6fe8c58c3707d6.png)

### Project 35：WIFI Station Mode

**1. Description**

ESP32 has three different WiFi modes: Station mode, AP mode and AP+Station mode. All WiFi programming projects must be configured with WiFi running mode before using, otherwise the WiFi cannot be used. In this project, we are going to learn the WiFi Station mode of the ESP32.

**2. Components**

<table class="colwidths-auto docutils align-default">
<tbody>
<tr class="odd">
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/729232b0c2d2c01984808289b222890c.png" style="width:1.8125in;height:0.86458in" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/53f17b0de2d98d4714e8fe9043a346ca.jpeg"  /></td>
</tr>
<tr class="even">
<td>USB Cable x1</td>
<td>ESP32*1</td>
</tr>
</tbody>
</table>

**3. Wiring Diagram**

Plug the ESP32 to the USB port of your PC

![](media/image-20230602171720765.png)

**4. Component Knowledge**

**Station mode：**

When setting Station mode, the ESP32 is taken as a WiFi client. It can connect to the router network and communicate with other devices on the router via a WiFi connection. As shown in the figure below, the PC and the router have been connected. If the ESP32 wants to communicate with the PC, the PC and the router need to be connected.

![](media/f74baff97695aa2ee33a8c19370d2547.png)

**5. Test Code**

![](media/01309c701d6fcf4f443076f8cacdffa1.png)


```Python
import time
import network # Import network module.

ssidRouter     = 'ChinaNet-2.4G-0DF0' # Enter the router name
passwordRouter = 'ChinaNet@233' # Enter the router password

def STA_Setup(ssidRouter,passwordRouter):
    print("Setup start")
    sta_if = network.WLAN(network.STA_IF) # Set ESP32 in Station mode.
    if not sta_if.isconnected():
        print('connecting to',ssidRouter)
  # Activate ESP32’s Station mode, initiate a connection request to the router
  # and enter the password to connect.      
        sta_if.active(True)
        sta_if.connect(ssidRouter,passwordRouter)
  #Wait for ESP32 to connect to router until they connect to each other successfully.      
        while not sta_if.isconnected():
            pass
  # Print the IP address assigned to ESP32-WROVER in “Shell”. 
    print('Connected, IP address:', sta_if.ifconfig())
    print("Setup End")

try:
    STA_Setup(ssidRouter,passwordRouter)
except:
    sta_if.disconnect()
```


**6. Test Result**

Since the router name and password are different in various places, so before running the code, the user needs to enter the correct router name and password in the red box shown above.

After entering the correct router name and password, click![](media/da852227207616ccd9aff28f19e02690.png)“Run current script”, the code will start
executing.

The Shell monitor will print the IP address of the ESP32 when connecting the ESP32 to your router.

![](media/e283d185859ce0a4372c53449bfd03b8.png)

### Project 36：WIFI AP Mode

**1. Description**

In this project, we are going to learn the WiFi AP mode of the ESP32.

**2. Components**

<table class="colwidths-auto docutils align-default">
<tbody>
<tr class="odd">
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/729232b0c2d2c01984808289b222890c.png" style="width:1.8125in;height:0.86458in" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/53f17b0de2d98d4714e8fe9043a346ca.jpeg" /></td>
</tr>
<tr class="even">
<td>USB Cable x1</td>
<td>ESP32*1</td>
</tr>
</tbody>
</table>

**3. Wiring Diagram**

Plug the ESP32 mainboard to the USB port of your PC

![](media/image-20230602171720765.png)

**4. Component Knowledge**

**AP Mode:**

When setting AP mode, a hotspot network will be created, waiting for other WiFi devices to connect. As shown below;

Take the ESP32 as the hotspot, if a phone or PC needs to communicate with the ESP32, it must be connected to the ESP32's hotspot. Communication is only possible after a connection is established via the ESP32.

![](media/35d90f1ce10814ea1897ba63f8bd7ad9.png)

**5. Test Code**

![](media/034021f83b237c1264e4677a784b4c2b.png)


```Python
import network #Import network module.

#Enter correct router name and password.
ssidAP         = 'ESP32_Wifi' #Enter the router name
passwordAP     = '12345678'  #Enter the router password

local_IP       = '192.168.1.147'
gateway        = '192.168.1.1'
subnet         = '255.255.255.0'
dns            = '8.8.8.8'

#Set ESP32 in AP mode.
ap_if = network.WLAN(network.AP_IF)

def AP_Setup(ssidAP,passwordAP):
    ap_if.ifconfig([local_IP,gateway,subnet,dns])
    print("Setting soft-AP  ... ")
    ap_if.config(essid=ssidAP,authmode=network.AUTH_WPA_WPA2_PSK, password=passwordAP)
    ap_if.active(True)
    print('Success, IP address:', ap_if.ifconfig())
    print("Setup End\n")

try:
    AP_Setup(ssidAP,passwordAP)
except:
    print("Failed, please disconnect the power and restart the operation.")
    ap_if.disconnect()
```


**6. Test Result**

You can modify the AP name and password or keep them unchanged

Click ![](media/c005d91eb85d5c58566746609ab80254.png)“Run current script”, the code will start executing. Open the AP function of the ESP32, the Shell monitor will
print the information.

![](media/5be2d032c8adcb2976c1640268919790.png)

Turn on your phone's WiFi search function, then you can see the ssid\_AP which is called "ESP32\_Wifi" in this code. You can enter the password "12345678" to connect it, or you can modify its AP name and password by code.

![](media/3e0ad895bea7f5100cc02a415adcace7.png)

### Project 37：WIFI AP+Station Mode

**1. Description**

In this project, we are going to learn the AP+Station mode of the ESP32.

**2. Components**

<table class="colwidths-auto docutils align-default">
<tbody>
<tr class="odd">
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/729232b0c2d2c01984808289b222890c.png" style="width:1.8125in;height:0.86458in" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/53f17b0de2d98d4714e8fe9043a346ca.jpeg" /></td>
</tr>
<tr class="even">
<td>USB Cable x1</td>
<td>ESP32*1</td>
</tr>
</tbody>
</table>

**3. Wiring Diagram**

Plug the ESP32 mainboard to the USB port of your PC

![](media/image-20230602171720765.png)

**4. Component Knowledge**

**AP+Station mode**

In addition to the AP mode and the Station mode, **AP+Station mode** can be used at the same time. Turn on the Station mode of the ESP32, connect it to the router network, and it can communicate with the Internet through the router. Then turn on the AP mode to create a hotspot network. Other WiFi devices can be connected to the router network or the hotspot network to communicate with the ESP32.

**5. Test Code**

![](media/f2e9eeb897d65975510976b3e178d695.png)


```Python
import network #Import network module.

ssidRouter     = 'ChinaNet-2.4G-0DF0' #Enter the router name
passwordRouter = 'ChinaNet@233' #Enter the router password

ssidAP         = 'ESP32_Wifi'#Enter the AP name
passwordAP     = '12345678' #Enter the AP password

local_IP       = '192.168.4.147'
gateway        = '192.168.1.1'
subnet         = '255.255.255.0'
dns            = '8.8.8.8'

sta_if = network.WLAN(network.STA_IF)
ap_if = network.WLAN(network.AP_IF)
    
def STA_Setup(ssidRouter,passwordRouter):
    print("Setting soft-STA  ... ")
    if not sta_if.isconnected():
        print('connecting to',ssidRouter)
        sta_if.active(True)
        sta_if.connect(ssidRouter,passwordRouter)
        while not sta_if.isconnected():
            pass
    print('Connected, IP address:', sta_if.ifconfig())
    print("Setup End")
    
def AP_Setup(ssidAP,passwordAP):
    ap_if.ifconfig([local_IP,gateway,subnet,dns])
    print("Setting soft-AP  ... ")
    ap_if.config(essid=ssidAP,authmode=network.AUTH_WPA_WPA2_PSK, password=passwordAP)
    ap_if.active(True)
    print('Success, IP address:', ap_if.ifconfig())
    print("Setup End\n")

try:
    AP_Setup(ssidAP,passwordAP)    
    STA_Setup(ssidRouter,passwordRouter)
except:
    sta_if.disconnect()
    ap_if.idsconnect()
```


**6. Test Result**

Before running the code, you need to modify ssidRouter, passwordRouter, ssidAP, and passwordAP. After making sure that the code is modified correctly, click ![](media/da852227207616ccd9aff28f19e02690.png)“Run current script” and the "Shell" window will display the following:

![](media/72c864c57de3f40d2a55ee3c10449898.png)

Then you can see the ssid\_A on the ESP32

![](media/3e0ad895bea7f5100cc02a415adcace7.png)

### Project 38: Comprehensive Experiment

![](media/c92bfcbd1ecd7fe91198066d0c9a4df6.jpeg)

**1. Introduction**

We did a lot of experiments, and for each one we needed to re-upload the code, so can we achieve different functions through an experiment? In this experiment, we will use an external button module to achieve different function.

**2. Components Required**

<table class="colwidths-auto docutils align-default">
<tbody>
<tr class="odd">
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/c9020c6015e55923afec197ab9d03fae.png" style="width:1.05278in;height:0.48819in" alt="4" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/6d96c844b0260ad712130945d692a7a2.jpeg" style="width:1.34444in;height:1.02986in" alt="ks0465-1" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/f0ef7a5a2e7eebb09e91f73cb2a6caf3.png" style="width:1.27292in;height:0.89722in" alt="白色LED模块" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/1aafa8910f5184973f1c913c19489fbd.png" style="width:1.27708in;height:0.90347in" alt="单路按键模块" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/a0eebfcd8f84c3fbac526e9910e66692.png" style="width:1.26319in;height:0.88472in" alt="旋转电位器传感器" /></td>
</tr>
<tr class="even">
<td>ESP32 Board*1</td>
<td>ESP32 Expansion Board*11</td>
<td>Keyestudio White LED Module*1</td>
<td>Keyestudio Button Module*1</td>
<td>Keyestudio Rotary Potentiometer*1</td>
</tr>
<tr class="odd">
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/b62846d9a80a7e7aed5ffbef0caedf7c.png" style="width:1.24167in;height:0.92083in" alt="避障传感器" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/fb4fa5fdd5689ded9c213ba5ceb34c0d.png" style="width:1.24097in;height:0.71319in" alt="摇杆模块" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/4a358f0f161b2e4dcae43f9315902ef3.png" style="width:1.27847in;height:0.63958in" alt="超声波模块" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/51729b3ba2184cf0ca0d3242199731ad.png" style="width:1.25972in;height:0.88125in" alt="共阴RGB模块" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/edbfec59fe015bd9987e4b4d542b466d.png" style="width:1.07361in;height:0.42778in" alt="USB线" /></td>
</tr>
<tr class="even">
<td>Keyestudio Obstacle Avoidance Sensor*1</td>
<td>Keyestudio DIY Joystick Module*1</td>
<td>Keyestudio HC-SR04 Ultrasonic sensor *1</td>
<td>Keyestudio DIY Common Cathode RGB Module *1</td>
<td>MicroUSB Cable*1</td>
</tr>
<tr class="odd">
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/0d81e07a0f67700c5a396fc7e1e614e1.jpeg" style="width:1.10069in;height:0.40069in" alt="3p线" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/269c154eda332be03643bada56070124.jpeg" style="width:1.14722in;height:0.44722in" alt="4p线" /></td>
<td><img src="https://raw.githubusercontent.com/keyestudio/KS5007-KS5008-Keyestudio-ESP32-24-in-1-Sensor-Kit-Python/master/media/fc3fd9c0110b04d1af77a2ff8c01a10a.png" style="width:1.10417in;height:0.46319in" alt="5p线" /></td>
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



