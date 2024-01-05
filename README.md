# Multiple-leds-using-finger-with-CVZONE-on-Arduino
CVzone is a computer vision package that makes us easy to run like face detection, hand tracking, pose estimation, etc., and also image processing and other AI functions. At the core, it uses OpenCV and MediaPipe libraries.

<img src="https://github.com/busolbuse/Multiple-leds-using-finger-with-CVZONE-on-Arduino/assets/147637348/1a43a3b7-4853-4d07-8b66-862930ea9a8c" alt="images"  width="500" height="300">

# What is pyFirmata?

Firmata is a protocol developed for computer software to communicate with microcontrollers. Using this protocol, we enabled our Python script to communicate with Arduino.

# Python and Arduino Communication by pyFirmata

<img src="https://github.com/busolbuse/Multiple-leds-using-finger-with-CVZONE-on-Arduino/assets/147637348/e08c1dc9-65e6-4140-9db6-83117c3176e7" alt="images"  width="250" height="200">

We transferred the codes in the Standard Firmata.ino file from the Firmata library, which we installed in the Arduino IDE, to the Arduino card and established communication with our Python code by establishing a bridge.

# How many fingers are on the screen?

<img src="https://github.com/busolbuse/Multiple-leds-using-finger-with-CVZONE-on-Arduino/assets/147637348/3f178cc4-9dd2-44e4-9b7b-e7c18158b268" alt="images"  width="500" height="300">

In our bridged python code, firstly the fingers were detected, the joints were determined, they were transferred to the matrix plane and the data in the matrix was examined. After this stage, the number of fingers shown on the screen is detected according to the matrix coordinate values. This detected value is written to the screen in the frame.exe file running as " Finger count: ".


