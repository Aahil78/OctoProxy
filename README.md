# OctoProxy

OctoProxy is a raspberry pi based OctoPrint server for the Bambu Lab A1, it acts as a proxy for region locked and LAN Only mode printers to have remote monitoring and access. It also has a Tailscale VPN server to trick Bambu Studio to think you are on  your LAN when you arent, this will allow you to send prints from Bambu Studio to any LAN Only printer from anywhere in the world. You can also use it as a printago fuse or simplyprint server.

Features:
  - Runs OctoPrint allowing you to send prints from anywhere.
  - Uses a Raspberry Pi 4 as the SBC, allowing for upgrades like sensors, lights, software upgrades, and more.
  - WS2812B/SK6812 3 Pin connector for custom lights.
  - Has a CSI Camera, allowing better timelapses and better video streaming footage. We all know the A1 Camera is..... special.
  - GPIO Pins broken out for upgrades.

## Images

### PCB:
<img width="1440" height="1054" alt="image" src="https://github.com/user-attachments/assets/bbab714e-74db-4fb0-aefb-3daf66374c3c" />
<img width="1699" height="1084" alt="image" src="https://github.com/user-attachments/assets/7107c06c-e32b-4381-99c1-ce3dc657299d" />

### Case:
<img width="1556" height="1167" alt="image" src="https://github.com/user-attachments/assets/964c9767-40d0-4c82-a675-a0168e937b2c" />
<img width="1800" height="1205" alt="image" src="https://github.com/user-attachments/assets/2f22fe09-bcad-4b63-8c53-d9ac604cf1ac" />
<img width="2118" height="863" alt="image" src="https://github.com/user-attachments/assets/c1a7b3af-a270-46c2-8e9e-70dc757f51ea" />

<img width="2055" height="1124" alt="image" src="https://github.com/user-attachments/assets/c6940ed3-d306-435b-8c6f-49b9d73670cd" />
(Top has magnets embedded)

### Schematic:
<img width="1846" height="287" alt="image" src="https://github.com/user-attachments/assets/5763dba7-8a62-4307-915a-e173999d2f77" />
<img width="870" height="653" alt="image" src="https://github.com/user-attachments/assets/1a4a2d65-ee04-4a6b-a1b1-d3e03dcc454d" />

## BOM:

1x Raspberry Pi
1x Raspberry Pi CSI Camera
1x PCBA
10x 3x2mm disc magnets
1x 3D Printed Case
1x Raspberry Pi Fan
Some screws and nuts
Spacers and standoffs
