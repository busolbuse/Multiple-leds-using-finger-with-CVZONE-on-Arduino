# Multiple-leds-using-finger-with-CVZONE-on-Arduino

# Purpose

Our aim in this project is to detect the behavior of fingers using Opencv and integrate it with the pyfirmata library and run it in the physical environment. This will be the basis of human-robot interaction in future projects. Our general goal is to understand the transfer of computer vision to the field of robotics.

CVzone is a computer vision package that makes us easy to run like face detection, hand tracking, pose estimation, etc., and also image processing and other AI functions. At the core, it uses OpenCV and MediaPipe libraries.

<img src="https://github.com/busolbuse/Multiple-leds-using-finger-with-CVZONE-on-Arduino/assets/147637348/1a43a3b7-4853-4d07-8b66-862930ea9a8c" alt="images"  width="500" height="300">

# What is pyFirmata?

Firmata is a protocol developed for computer software to communicate with microcontrollers. Using this protocol, we enabled our Python script to communicate with Arduino.

# Python and Arduino Communication by pyFirmata

We transferred the codes in the Standard Firmata.ino file from the Firmata library, which we installed in the Arduino IDE, to the Arduino card and established communication with our Python code by establishing a bridge.


# How many fingers are on the screen?

<img src="https://github.com/busolbuse/Multiple-leds-using-finger-with-CVZONE-on-Arduino/assets/147637348/3f178cc4-9dd2-44e4-9b7b-e7c18158b268" alt="images"  width="500" height="350">

In our bridged python code, firstly the fingers were detected, the joints were determined, they were transferred to the matrix plane and the data in the matrix was examined. After this stage, the number of fingers shown on the screen is detected according to the matrix coordinate values. This detected value is written to the screen in the frame.exe file running as <b><i>" Finger count: "</i></b>.


# Data transfer from one python to another python and arduino-led communication 

By importing the <b><i>"pyFirmata"</i></b> library into our Python code, we transferred data from Python to Arduino for controls. At this stage, after selecting the board with the functions contained in the library and specifying the compor part as the USB input we plugged in, the data received from the other python code of the LEDs was processed. We defined which pin the LEDs were plugged into in Arduino with the <b><i>"get_pin"</i></b> function.
We set the data coming to our code to be a 1x5 matrix. Then, we explained how many LEDs would light this matrix data in the Python script with if else condition statements.
Arduino software was written using the Python code, Visual Studio Code compiler, where the pin inputs of the LEDs were defined.

<img src="https://github.com/busolbuse/Multiple-leds-using-finger-with-CVZONE-on-Arduino/assets/147637348/6e30191d-fee9-457e-a6c9-32fb3c7f381f" alt="images"  width="500" height="300">

https://github.com/busolbuse/Multiple-leds-using-finger-with-CVZONE-on-Arduino/assets/147637348/177b417c-df62-455d-92e4-e07cfee0015e

# Requirements:

Arduino Uno 

Breadboard
 
5 different colors LED

Male to male cable 

USB A to USB B cable

# Authorises:

Buse Berren Ünal

Zeynep Çapak

# References:
[1] https://github.com/tino/pyFirmata

[2] https://github.com/cvzone/cvzone