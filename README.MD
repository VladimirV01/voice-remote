# Voice Remote for Home Assistant
This is a ESPHome based device which can interact with voice assistants configured in Home Assistant. 

![Assembly](Renders/Assembly_Exploded_View.png "Assembly Exploded View" )

## Project Timeline
Initially, I thought about this kind of project when I saw [$13 voice remote for Home Assistant](https://www.home-assistant.io/voice_control/thirteen-usd-voice-remote/) article. 

I tried to buy one **M5Stack ATOM Echo Development Kit**, but at that time it was out of stock almost everywhere I looked and it was pretty hard to source in my country. As a result, this idea transitioned to PENDING state until I manage to get an M5Stack or find a different approach. 

Some time later, thanks to the gods of youtube algorithms :smile:, I found a [video](https://www.youtube.com/watch?v=EeUG3Si9fZk) where the author describes very well an alternative for the **M5Stack ATOM kit** using **ESP32** based development board called **Adafruit Feather v2 ESP32 board**, which again was not very easy to find and source from my country.


So I decided to make my own adaptation of the project using plain ESP32 module and a custom PCB, because I like to design PCBs and I like when my projects are nice and tidy. 

___

### Main Components
- ESP32-WROOM Module
- INMP441 I2S MEMS Microphone Module
- MAX98357A I2S Amplifier
- TPS63020 Buck-Boost Converter Module
- WS2812 Addressable LED
- A tactile switch that you like (I used B3F-4055)
- A small speaker of your choice (I used AS02008MR)
- TP4056 Li-Ion Charging Module
- A Li-Ion battery (I used one from an old iPhone due to the form factor)
- Other miscellaneous components like SMD Resistors, Capacitors, etc.
___
### Case
![Case](Renders/Case.png "The Case")
The case can be printed on a 3D printer without using any support, the files are attached in the "Case STL" folder. 

Also [here](https://cad.onshape.com/documents/a099e547f9d236687422ab01/w/ca8a76f6cc6eaf7c9584012f/e/bb01b9a7f8b48ed9828aac3d) is the link to the OnShape project. Anybody can make a copy and edit it if you want to make some changes to the case that will better suit your use-case.
___

### PCB
The printed circuit board was designed by me and I manufactured it using JLCPCB services and it turned out amazing. 
![PCB](Photos/PCB.jpg "Printed Circuit Board")
And here is it assembled.
![Assembled PCB](Photos/PCB_Top_View.jpg "Assembled Printed Circuit Board")
___
### TO DO:
- Design a case adaptation for 18650 Li-Ion battery
- Remove the strapping pins (12, 15) to please my internal perfectionist and ESPHome code checker.
- Add Links to BOM

