[🇷🇺 Русская версия документации здесь](https://github.com/renat2985/bitball.club/blob/main/README_RU.md)

# Smart Fight Ball (Box Ball) Based on ESP8266

<a href="https://www.youtube.com/watch?v=Eb2ycZCe_rk&list=PL6NJTNxbvy-JwHCaki6eOuAYkdLQA4lqW"><img src="https://github.com/renat2985/bitball.club/blob/main/doc/bitball3.png"></a>

This is an advanced version of the classic elastic ball game (Box Ball), designed to improve coordination, reaction speed, and agility. Unlike a standard ball, our device is equipped with smart electronics based on the ESP8266 microcontroller (NodeMCU). It can track the number of hits, measure hit force, and enable online competition via the [bitball.club](https://www.bitball.club) website with other users who have similar devices. Players can also track their progress in real-time.

You can build the device yourself or ask us to do it for you. To order a ready-made device, contact us via [Telegram](https://t.me/ESPiotDevice), [Skype](https://skype:renat2985?chat), or [Discord](https://discord.com/invite/zaGaDuGe).

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

      <img src="https://github.com/renat2985/bitball.club/blob/main/doc/WiFi.png" width="200px">

3. Access the game through a browser:
   - Open a browser and enter the address: `http://192.168.4.1`.

      <img src="https://github.com/renat2985/bitball.club/blob/main/doc/AP.gif" width="300px">

#### **Tip**: If you connect BitBall to your router, you won’t need to reconnect to BitBall.club Wi-Fi each time. Simply visit [www.bitball.club](https://bitball.club), and you’ll enter the game instantly. Plus, you’ll be able to save your training results, compete with others online, and enjoy various other features.

## HTTP and Security

Our device uses WebSocket without SSL, which makes it incompatible with HTTPS. As a result, we had to keep the domain accessible via HTTP only.
However, this does not affect your security in any way, as the site does not require passwords or any other sensitive information.

<img src="https://github.com/renat2985/bitball.club/blob/main/doc/security.gif" width="500px">


## Wiring Diagrams

### Basic
NodeMCU ESP8266, Wemos ESP8266

<img src="https://github.com/renat2985/bitball.club/blob/main/doc/schematic/schematicEasy.png" width="300px"> <img src="https://github.com/renat2985/bitball.club/blob/main/doc/schematic/schematicWemosEasy.png" width="300px">

### Advanced
NodeMCU ESP8266, Wemos ESP8266

<img src="https://github.com/renat2985/bitball.club/blob/main/doc/schematic/schematic.png" width="300px"> <img src="https://github.com/renat2985/bitball.club/blob/main/doc/schematic/schematicWemos.png" width="300px">

## STL (3d print folder)
This backing is essential for the correct operation of the weight sensor; without it, false triggers may occur. It’s important that the internal part of the scale does not come into contact with the forehead or any other surfaces.

<img src="https://github.com/renat2985/bitball.club/blob/main/3d%20print/sensorBox.png" height="300px"> <img src="https://github.com/renat2985/bitball.club/blob/main/3d%20print/sensorBoxAUX.png" height="300px"> 

## Components

<img src="https://github.com/renat2985/bitball.club/blob/main/doc/components/canva.png" height="300px"> <img src="https://github.com/renat2985/bitball.club/blob/main/doc/IMG_9764.png" width="400px"> <img src="https://github.com/renat2985/bitball.club/blob/main/doc/IMG_9752.png" width="400px">


## From AliExpress.com

<sup>https://www.aliexpress.com/item/1005004893349830.html - NodeMCU ESP8266</sup>

<sup>https://www.aliexpress.com/item/1005006293517345.html - Weight Sensors + HX711</sup>

<sup>https://www.aliexpress.com/item/32556525207.html - ULN2003A</sup>

<sup>https://www.aliexpress.com/item/1005002060362335.html - Nylon Elastic Band</sup>

<sup>https://www.aliexpress.com/item/4000977316378.html - Elastic Band Round</sup>

<sup>https://www.aliexpress.com/item/1005002367815544.html - Power Bank (for 18650 Battery) </sup>

<sup>https://www.aliexpress.com/item/1005005898038310.html - Head Straps Headband</sup>



## 🚀 Web installer (recommended)

### Go to the web installer and follow instructions.

### [https://renat2985.github.io/bitball.club/](https://renat2985.github.io/bitball.club/)


## :battery: Donation

If you like this project, you can buy me a cup of coffee :coffee:

<img src="https://github.com/renat2985/renat2985/raw/main/donate/donate.png" width="100%">

- PayPal [https://www.paypal.me/RKevrels](https://www.paypal.me/RKevrels/5)