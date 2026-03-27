### Project 1: Hello World

**1. Overview**

For ESP32 beginners, we will start with some simple things. In this project, you only need a ESP32 mainboard, a USB cable and a computer to complete the "Hello World\!" project, which is a test of communication between the ESP32 mainboard and the computer as well as a primary project.

**2. Components**

| ![image-20231113151026574](media/image-20231113151026574.png) | ![image-20231113151032312](media/image-20231113151032312.png) |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| ESP32*1                                                      | USB Cable*1 

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

In the new dialog box，select“Project\_01\_HelloWorld.py”,click“Open”. The code used in this tutorial is saved in the file **MicroPython\\ESP32\_code\_MicroPython**. You can move the code to anywhere, for example, we can save the**ESP32\_code\_MicroPython in the** Disk(D), the route is <span style="color: rgb(255, 76, 65);">**D:\\2.ESP32\_code\_MicroPython.**</span>（The code in this tutorial is saved in the Disk(D) on your computer）

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
