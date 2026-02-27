# February 26th, 05:20pm : Brainstormed the idea and made the schematic

Hi! I recently got a Bambu Lab A1 from [Construct](https://construct.hackclub.com) (An event where you do 40hrs of 3D CAD to get an A1 Mini, do 70hrs and get an A1!! Ages 13-18) but it was region locked as only the A1 CN Version was available over here. So I thought, why not make an upgrade for my printer? So I brainstormed this project. 

---
Features:
  - Runs OctoPrint allowing you to send prints from anywhere.
  - Uses a Raspberry Pi 4 as the SBC, allowing for upgrades like sensors, lights, software upgrades, and more.
  - WS2812B/SK6812 3 Pin connector for custom lights.
  - Has a CSI Camera, allowing better timelapses and better video streaming footage. We all know the A1 Camera is..... special.
  - GPIO Pins broken out for upgrades.
  - Uses a DSI Touchscreen for print stats/different control panel.
---
So after thinking abt all of this, I created a schematic in KiCad with the following broken out: 
  - ARGB LED Strip 3pin connector (330ohm on Data line - Data Line tied to GPIO18)
  - I2C Breakout
  - SPI Breakout
  - Fan Breakout (2pins to 5v and GND)
  - PWM Pins GPIO12, 13, and 19
  - Input Pins GPIO4, 5, 6, 17, 23, and 24
  - Output Pins GPIO20, 21, 22, 25, 26, and 27
  - General Pin Broken Out GPIO16
  - UART Pins - TX, RX, 3.3v, and GND.
  - Power Pins - GND, 3.3v, and 5v

I'll make a PCB now then work on the enclosure.

<img width="2617" height="1839" alt="image" src="https://github.com/user-attachments/assets/dcfc0ea1-5250-4f0d-a314-26a2cb52cdc8" />
<img width="2704" height="401" alt="image" src="https://github.com/user-attachments/assets/9e5b2beb-c061-4979-bfc6-0f29b6504299" />

**Total time spent: 3h**


# February 26th, 06:18pm : Changed the schematic

Okay so I was assigning footprints and found out I don't have a footprint for the Pi HAT with cutouts for DSI and CSI cables, so i made a new project with the "Raspberry Pi HAT" Template on KiCad and copy pasted everything then put all the Net Labels to the correct pins.

<img width="1860" height="1411" alt="image" src="https://github.com/user-attachments/assets/b60368b8-5922-46bf-99f9-ec7674244b87" />

**Total time spent: 58mins**

# Fubruary 26th, 08:00pm : Made the PCB

Soooo, I made the PCB!!! It was pretty hard to arrange all the components in a limited space, now I'm gonna work on the enclosure.

<img width="2379" height="1576" alt="image" src="https://github.com/user-attachments/assets/f5e68d6e-96e2-4f0f-80ce-c002435981ef" />

**Total time spent: 1hr 42mins**

# February 28th, 01:15am : Labled all pins

So I went over and exported the 3D Model of the PCB and noticed I didnt label any of the pins, so I did that rn. I didnt do the ones on the side cz theres no space and they may not be used that much, might label those on the enclosure if I can.

<img width="2127" height="1564" alt="image" src="https://github.com/user-attachments/assets/6e2a3853-20ba-42e8-98fd-aca185600dbc" />

**Total time spent: 15mins**

# February 28th, 03:45am : Populated the PCB

Sooo I researched all the components, shortlisted them, decided the final components, downloaded it's 3D Model, imprt it, then position it onto my PCB in the assembly. Now I'll export the populated PCB+Raspberru Pi then make my sketch around that.

<img width="2859" height="1541" alt="image" src="https://github.com/user-attachments/assets/486d8a86-01ca-4cf3-a43c-5c2eb37d71a9" />

**Total time spent: 3hrs 30mins**
