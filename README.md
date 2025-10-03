# ESP32-CAM Virtual Mouse

A **virtual mouse** using the **ESP32-CAM module** that allows you to control your computer cursor using hand gestures or camera input.

## Key Features
- Control your mouse pointer using ESP32-CAM module  
- Click and scroll gestures supported  
- Lightweight and portable hardware solution  
- Ideal for IoT, robotics, and gesture-controlled applications  

## Technologies Used
- ESP32-CAM
- FTDI Module
- Arduino IDE
- Python 
- OpenCV or simple image processing for gesture detection (if used)  
- WiFi Connection 

## Hardware Setup
1. ESP32-CAM module  
2. FTDI programmer (for flashing code)    

Connection [https://github.com/azharajju875/ESP32CAM-Virtual-Mouse/blob/main/ESP32-CAM%20and%20FTDI.png]

## Code Usage
1. Open Arduino IDE go to flie -> exampkes -> esp32 -> camera -> camerawebserver
2. A code will be generated just comment the #define camera model wover kit and uncomment #define camera madel AI thinker
3. Put the WiFi credentials which is connected to your computer
4. Upload the code
5. After code is uploaded disconnect the GPIO pin and Ground pin in board and press the reset button on the board
6. Check the serial monitor an URL will be generated copy that and paste in any browser and check for video streaming
7. Now open Python paste the HandTracking code [https://github.com/azharajju875/ESP32CAM-Virtual-Mouse/blob/main/HandTrack], this code used to track your hand through laptops camera andcontrol the cursor on screen
8. If everything works good till here create another file and paste the Final code [https://github.com/azharajju875/ESP32CAM-Virtual-Mouse/blob/main/Final], in this code simply code the URL generated in the Serial monitor of Arduino IDE after URL and after the URL add /capture and click on run.
9. Now the cursor will be controlled by your hand gesture through ESP32-CAM.
