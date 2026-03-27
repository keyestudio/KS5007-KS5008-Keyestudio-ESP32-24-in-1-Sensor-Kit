## Arduino Development Environment Configuration

### Windows System：

![](media/6cf6312dc7c7db27794b54d58a8bf80c.png)

#### 1.1 Installing Arduino IDE

⚠️ **Special reminder: ** The Arduino IDE version used in this tutorial is 1.8.16. If it is a different version, there is no guarantee that the sample code provided in this tutorial will compile and upload successfully.

When you get control board, you need to download Arduino IDE and driver firstly.

You could download Arduino IDE from the official website:[<span class="underline">https://www.arduino.cc/</span>](https://www.arduino.cc/), click the “SOFTWARE”on the browse bar, then click<span class="underline">“DOWNLOADS”</span> to enter download page, as shown below:

![](media/bfe8c9e405c71123dee7921eddff86d3.png)

![](media/7250961db41ba42e4b881d77bd76a319.png)

There are various versions of IDE for Arduino. Just download a version compatible with your system. Here we will show you how to download and install the windows version of Arduino IDE.

![](media/894116c5cf0023dd9720946cfb441790.png)

There are two versions of IDE for Windows system: Windows Win7 and newer and Windows ZIP file. The former needs to install manually, while the latter can be directly downloaded, without the need of installing it manually.

![](media/a983a2f2eceb968afbff8ba0f0376240.png)

You just need to click JUST DOWNLOAD.

After the Arduino is downloaded, click“I Agree”to continue installing and click **Next.**

![](media/00e334d3c756a2495da6f0d1b2db680a.png)

![](media/de541d90a1cda992ad8e3f0cbaf95f94.png)

Then click **Install.**

![](media/7da9aca1e8432c59372e7c7ab2574bd9.png)

If the following page appears, click **Install.**

![](media/85b29de2aa791ecc77280ccde91e53c5.png)

![](media/739c41701fbcab202f0e587f534bad30.png)

![](media/d28223c55a30f949760779720fe4ec24.png)

#### 1.2 Install a driver on Windows

If you have installed the driver, just skip it.

Before using the ESP32 board, you must install a driver, otherwise it will not communicate with computer.

Unlike the USB series chip (ATMEGA8U2) of the Arduino UNO R3, the ESP32 board uses the CP2102 chip USB series chip and USB type C interface.

The driver of the CP2102 chip is included in 1.8.0 version and newer version of Arduino IDE. Usually, you connect the board to the computer and wait for Windows to begin its driver installation process. After a few moments, the process will succeed.

If the driver installation process fail, you need to install the driver manually.

**Note:**

1\. Please make sure that your IDE is updated to 1.8.0 or newer version.

2\. If the version of Arduino IDE you download is below 1.8, you should download the driver of CP2102 and install it manually.

Link to download the driver of CP2102: [**<span class="underline">https://fs.keyestudio.com/CP2102-WIN</span>**](https://fs.keyestudio.com/CP2102-WIN)

To install the drive manually, open the device manager of computer.

Right click Computer----- Click Properties-----Click Device Manager.

Look under Ports (COM & LPT) or other devices.

A yellow exclamation mark means that the CP2102 driver installation failed.

![](media/9af2e34bf9bdd6675bdf5fa8cd291971.png)

Double-click ![](media/a2455b26773cb8d6cb3fccc605ea4dd7.png) and click “ **Update drive...**”

![](media/a122cd6fef74eb5c0c7fe16fac2fed59.png)

Click“Browse my computer for drivers ” to find installed or downloaded Arduino software .  

![](media/a02d3e643231cfe267d4debf0ef258c4.png)

There is a DRIVERS folder in Arduino software installed package（![](media/aae89b3213589edf1c320d5502489820.png)), open driver folder and you can see the driver of CP210X series chips.

Click“Browse”to select the driver of CP210X series chips then click“Next”.

![](media/eb6ca318005b5c570ad4fbef73024351.png)

![](media/4f2af46602a5ef73985914170911c519.png)

Open device manager, you will find the yellow exclamation mark disappear. The driver of CP2102 is installed successfully.

![](media/af2324b73308f1796b8b7c9dc14878e7.png)

#### 1.3 Install the ESP32 on Arduino IDE

Note：you need to download Arduino IDE 1.8.5 or advanced version to install the ESP32.

1) Click![](media/4f2de68a91c7f59024aa87a522e36ab3.png)to open Arduino IDE
     
![](media/8aca9b5378e794375f2c15d3b4e238ba.png)

2) Click **“ File**” →**“Preferences”**，copy the website address <https://dl.espressif.com/dl/package_esp32_index.json> in
    the“**Additional Boards Manager URLs:**”and click“**OK**”.
    
![](media/a8febbd62268514a30cec4e183b1eaed.png)

![](media/ea68c66041f48b44b4682eb3a0e11e79.png)

3) Click“**Tools**”→“**Board:**”then click “**Boards Manager...**”to enter“**Boards Manager**”. Enter **ESP32**”as follows, then click
    **Install .**
    
⚠️ **Note:**  This tutorial uses the ESP32 development board version 1.0.6. Please keep it consistent to avoid code incompatibility issues.
    
![](media/a710d2a8166e3e62d9b48d9b7386e9e4.png)
    
![](media/9824059733dcbbfb3dff58736923a4a9.png)
    
(4) After installing, click“Close”

#### 1.4 Arduino IDE Setting

Click![](media/675ae7298ce0973df720b2fbbb514caa.png)icon to pen Arduino IDE.

![](media/8aca9b5378e794375f2c15d3b4e238ba.png)

When downloading the sketch to the board, you must select the correct name of Arduino board that matches the board connected to your computer. As shown below;

(Note: we use the ESP32 board in this tutorial; therefore, we select ESP32.)

![](media/78695faae974868fb29c972e89a9d917.png)

![](media/3a3bbc0ce1845aceb35af40aea7c84ca.png)

Set the board type as follows;

![](media/43b6c4d7f639f1e4b7adb017db805ea1.png)

Then select the correct COM port (you can see the corresponding COM port after the driver is successfully installed).

![](media/94587092f31929ebb9cdbcc5fe1718de.png)

![](media/97ab2e53b87bd0812b2b064405f86196.png)

![](media/1235ef274c17d00db74fca324072ff84.png)

A- Used to verify whether there is any compiling mistakes or not.

B- Used to upload the sketch to your Arduino board.

C- Used to create shortcut window of a new sketch.

D- Used to directly open an example sketch.

E- Used to save the sketch.

F- Used to send the serial data received from board to the serial monitor.

### Mac System

![](media/a6fc83596009c574d8e29ef383748549.png)

#### 2.1 Download Arduino IDE

![](media/5d58d3cf67b308423ddb9f286f6cb697.png)



⚠️ **Note:**  This tutorial uses the ESP32 development board version 1.0.6. Please keep it consistent to avoid code incompatibility issues.

#### 2.2 How to install the CP2102 driver

If you have installed the driver, just skip it.

Connect the ESP32 board to your computer, and open Arduino IDE.

Click **Tools→Board:ESP32 Dev Module and /dev/cu.usbserial-0001.**

![](media/00d823dbf27e569a2ba23277b1e15a41.jpeg)

Click ![](media/9c9158a5d49baa740ea2f0048f655017.png) to upload code.

Note: If code is uploaded unsuccessfully, you need to install the driver of CP2102, please continue to follow the instructions as below:

Download the driver of CP2102:

<https://www.silabs.com/products/development-tools/software/usb-to-uart-bridge-vcp-drivers>

Select Mac OSX edition, as shown below;

![](media/c09e7c279a858574756d1192b3a995aa.png)

Unzip the downloaded package.

![](media/6870a714ddd11015dc43b1d5743e0666.jpeg)

Open folder and double-click **SiLabsUSBDriverDisk.dmg** file.

![](media/61ae3e706a1c4afa7948d5fb2e797a6d.png)

You will view the following files as follows:

![](media/3f1afe9499f6d852492cfb9d6b11e9ab.jpeg)

Double-click “Install CP210x VCP Driver”, tick D**on’t warn me when opening application on this** **disk image** and tap “ **Open”.**

![](media/14f6ebb088e654abc2f0149645e34ed1.png)

Click“**Continue**”

![](media/b1cb125dccf6470ebe255f8f65b902eb.jpeg)

Tap **Agree,** and **Continue**

![](media/865dcc76cb7f58854b56f1020233f05e.jpeg)

Click **Continue** and input your password.

![](media/1ef6d65b61ad7c6e0a3989ba59de74d5.jpeg)

![](media/29bbca3360d806164717733460574356.png)

**Select** “**Select Open Security Preferences**”.

![](media/ca6bc6e536202f07a53c09201a0996ff.png)

Click the lock to unlock security & privacy preference.

![](media/cb6be428257143635fc4f729487549c5.jpeg)

![](media/e8f637a3a9510aa8f90c65820d4d1cd8.jpeg)

Tap **Unlock and** enter **your Username and password，**then click **Allow.**

![](media/250a1cbb7f93fc2a572944bea9fe5494.jpeg)

Back to installation page, and wait to install.

![](media/0da6d0d4296d6e3de0b30dfd3c615265.jpeg)

Successfully installed

![](media/7cca827fe946096f228797dadce10661.jpeg)

Then enter ArduinoIDE, click **Tools** and select Board **ESP32 Dev Module** and the serial port is“**/dev/cu.SLAB\_USBtoUAPT.**

![](media/00d823dbf27e569a2ba23277b1e15a41.jpeg)

Click![](media/b7c913eaa4dcea1bc326dd7a7b5a2af6.png) to upload code and show“Done uploading”.

![](media/16cee842865ba86e42468b67c17c415c.png)

### How to Add Libraries?

⚠️ **<span style="color: rgb(255, 76, 65);">Special Note:</span>** You can refer to the methods in the linked content to add the library files. click the link：[https://getting-started-with-arduino.readthedocs.io](https://docs.keyestudio.com/projects/Arduino/en/latest/Arduino%20IDE%20Tutorial.html#import-library)

**(1) What are Libraries ?**

[Libraries ](https://www.arduino.cc/en/Reference/Libraries)are a collection of code that make it easy for you to connect sensors, displays, modules, etc.

For example, the built-in LiquidCrystal library helps talk to LCD displays. There are hundreds of additional libraries available on the Internet for download.

The built-in libraries and some of these additional libraries are listed in the reference. (https://www.arduino.cc/en/Reference/Libraries)

**(2) How to Install a Library ?**

Here we will introduce the most simple way to add libraries .

**Step 1:** After downloading well the Arduino IDE, you can right-click the icon of Arduino IDE to find the option "Open file location" .

![](media/49c79c59250fa02d4fc4c2d8929ad274.png)

**Step 2:** Click **Open file location** \>libraries

![](media/2b05ac39b2ad481965c9384dd5347194.png)

![](media/89211927cafc8f4c735d72c87d9dc05e.png)

**Step 3:** Next, find out the“libraries”folder

![](media/fdb3ffba2e170acf83c96274aa1b21c2.png)

![](media/f01292302e4cbd954e8902d1ab359c40.png)

Copy ![](media/eb0f19c7cc3a1bbf84953dabe63ada92.png)in the libraries folder of Arduino.

Then click“Replace the files in the destination”.

![](media/48cc1fcf111ce12c3e174393eee4991d.png)

![](media/012eaa83ed77c061e20d6257f09a4e53.png)
                    

