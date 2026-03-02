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

# March 1st, 10:47am : Redid the PCB

So last night in Onshape, I found out the GPIO Header was mislaigned, so I had to delete all traces, replace the footprint to spaarkfun's PCM RPi Hat connector, and precisely aligned everything asw. I then routed everything again, I also added all 3D Models to the PCB this time to save time for later on.

<img width="2114" height="1542" alt="image" src="https://github.com/user-attachments/assets/870d42be-855f-4f33-9296-f7bae09c7e6f" />

<img width="2678" height="1778" alt="image" src="https://github.com/user-attachments/assets/9efde93a-72d9-4dbd-a8c1-cfed15386303" />

<img width="2307" height="1799" alt="image" src="https://github.com/user-attachments/assets/48ac27ce-2435-4950-9529-2c40b774dce6" />

**Total Time Spent: 2hrs 45mins**

# March 2nd, 10:07pm : Starting the case

I added the PCB and Pi in OnShape, connected them im an assembly, exported the assembly, added the export back into OnShape as a part studio, then I started off the case, aligned the Pi in it, and made cutouts for the Type C, HDMI, and audio port.

<img width="2174" height="1625" alt="image" src="https://github.com/user-attachments/assets/c54d88e1-d025-4cb1-824d-8f35ea2d2469" />
<img width="2077" height="1471" alt="image" src="https://github.com/user-attachments/assets/046e2c7b-2e92-4a9b-9682-bbabd15a9329" />

**Total time spent: 3hrs**

# March 3rd, 12:27am : Case bottom done

I made the whole bottom, added text, cutouts, fillets, etc. I'll make the top now, might use heatset inserts to screw in the top. (The top is really big cz I have to fit in a 2010 or 4010 fan too.)

<img width="1869" height="1587" alt="image" src="https://github.com/user-attachments/assets/0085d5f8-72d4-4956-a680-50f55ea7966e" />

**Total time spent: 2hr 20mins**

# March 3rd, 01:17am : Finished the case!

So im finally done with the case!! I'll use a different fan that screws onto the pi not case. and for the camera I'll use a stand I have at home, also for the LCD, I am not gonna add one because this is intended for a server, but if needed i can use the HDMI ports. I'll add all files then submit.

<img width="2140" height="1487" alt="image" src="https://github.com/user-attachments/assets/957d68cb-384b-449e-a19a-fc8604f02502" />

**Total time spent: 1hr**
