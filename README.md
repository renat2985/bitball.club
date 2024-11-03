# Smart Box Ball Based on ESP8266

![Smart Box Ball](https://github.com/renat2985/bitball.club/blob/main/doc/bitball2.png)

This is an advanced version of the classic elastic ball game (Box Ball), designed to improve coordination, reaction speed, and agility. Unlike a standard ball, our device is equipped with smart electronics based on the ESP8266 microcontroller (NodeMCU). It can track the number of hits, measure hit force, and enable online competition via the [bitball.club](https://bitball.club) website with other users who have similar devices. Players can also track their progress in real-time.

## Key Features
- **Hit Tracking**: The device uses built-in sensors to accurately record every hit on the ball.
- **Hit Force Calculation**: The device analyzes sensor data to measure hit force, adding a competitive edge.
- **Wi-Fi Connectivity**: The device connects to Wi-Fi, allowing players to save training results in the cloud and participate in online tournaments.
- **Flexible Training Settings**: Users can set training durations and other parameters, tailoring the device to personal goals.
- **Feedback System**: Sound or light alerts help signal training completion or motivate users to improve their results.
- **Online Competitions**: Players can compete in real-time with others via [bitball.club](https://bitball.club), compare results, and elevate their training.

## Benefits
- **Interactivity**: Training becomes more engaging and interactive thanks to automatic counting, hit force measurement, and instant feedback.
- **Real-Time Competitions**: Users can compete with others globally, making training even more exciting.

Our smart Box Ball is not just an elastic ball—it’s a high-tech training device that lets you set goals, track progress, measure hit force, and reach new heights in coordination and reaction training.

## Contact Information

You can assemble the device yourself or request a pre-assembled one. To order a ready-made device, contact me via [Telegram](https://t.me/ESPiotDevice), [Skype](https://skype:renat2985?chat), or [Discord](https://discord.com/invite/zaGaDuGe).

## Instructions

### Powering On the Device
- **First Signal**: The device has successfully powered on.
- **Second Signal (Charge Level Indication)**:
  - High tone — battery at 100%.
  - Medium tone — battery at 50%.
  - Low tone — battery at 25%. In this mode, sound is disabled to save energy.
- **Third Signal (Operating Mode after 4-15 seconds)**:
  - High tone — device connected to the router.
  - Low tone — connection to the router failed. The device has created a WiFi hotspot called "BitBall.club".

- **Auto Sleep Mode**: If the game has not started within 5 minutes, the device enters sleep mode. The sleep mode signal is a high tone that gradually lowers to a low tone.

### How to Start Playing with BitBall
1. Turn on the BitBall device.
2. Connect to Wi-Fi:
   - Select the BitBall.club network.
   ![Wi-Fi Connection](https://github.com/renat2985/bitball.club/blob/main/doc/WiFi.png)

3. Access the game through a browser:
   - Open a browser and enter the address: `http://192.168.4.1`.
   ![Browser Access](https://github.com/renat2985/bitball.club/blob/main/doc/AP.gif)

#### **Tip**: If you connect BitBall to your router, you won’t need to reconnect to BitBall.club Wi-Fi each time. Simply visit [www.bitball.club](https://bitball.club), and you’ll enter the game instantly. Plus, you’ll be able to save your training results, compete with others online, and enjoy various other features.

![BitBall](https://github.com/renat2985/bitball.club/blob/main/doc/bitball2.png)

## Wiring Diagrams

### Basic
NodeMCU ESP8266  
![Basic NodeMCU Schematic](https://github.com/renat2985/bitball.club/blob/main/doc/schematicEasy.png)

Wemos ESP8266  
![Basic Wemos Schematic](https://github.com/renat2985/bitball.club/blob/main/doc/schematicWemosEasy.png)

### Advanced
NodeMCU ESP8266  
![Advanced NodeMCU Schematic](https://github.com/renat2985/bitball.club/blob/main/doc/schematic.png)

Wemos ESP8266  
![Advanced Wemos Schematic](https://github.com/renat2985/bitball.club/blob/main/doc/schematicWemos.png)

## Components
![Components](https://github.com/renat2985/bitball.club/blob/main/doc/components/canva.png)

https://www.aliexpress.com/item/1005004893349830.html
https://www.aliexpress.com/item/1005006293517345.html
https://www.aliexpress.com/item/32556525207.html
https://www.aliexpress.com/item/1005002060362335.html
https://www.aliexpress.com/item/4000977316378.html
https://www.aliexpress.com/item/1005002367815544.html
https://www.aliexpress.com/item/1005005898038310.html



# For Advanced Users: Instructions for Flashing via Programmer

## Web installer (recommended)

## Go to the web installer and follow instructions.

## [https://renat2985.github.io/bitball.club/](https://renat2985.github.io/bitball.club/)


Specification of [bitball.build.bin](https://github.com/renat2985/bitball.club/raw/main/build/esp8266.esp8266.generic/bitball.build.bin) file
```
  -  Module: Generic ESP8266 Module
  -  Flash Size: 1M
  -  CPU Frequency: 80Mhz
  -  Flash Mode: DOUT
  -  Flash Frequency: 40Mhz
  -  Upload Speed: 921600
```

### NodeMCU Flasher
https://github.com/nodemcu/nodemcu-flasher
Download Release: [Win32](https://github.com/nodemcu/nodemcu-flasher/blob/master/Win32/Release/ESP8266Flasher.exe) or [Win64](https://github.com/nodemcu/nodemcu-flasher/blob/master/Win64/Release/ESP8266Flasher.exe).

## :battery: Donation

If you like this project, you can buy me a cup of coffee :coffee:

<img src="https://github.com/renat2985/toncoin_payment/blob/main/doc/donate.png" width="700px">

- PayPal [https://www.paypal.me/RKevrels](https://www.paypal.me/RKevrels/5)