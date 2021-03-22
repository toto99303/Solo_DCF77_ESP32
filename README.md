# Solo DFC77 ESP32 transmitter
So what is this? It's a standalone DCF77 transmitter designed to be used with any wrist watch that is capable of receiving the signal. (Casio Wave Ceptor series etc.)

#### Features:
- Connects to your local WiFi network.
- Syncs the exact time via NTP and converts it to DCF77 signal.
- Shows the realtime data on the OLED display live.
- Uses screensavers to protect the screen from burn-in. (changes every minute)
- 3D printable stand.

![](https://github.com/toto99303/Solo_DCF77_ESP32/blob/main/Pictures/ready1.jpg)

### PCB and full BOM:

![](https://github.com/toto99303/Solo_DCF77_ESP32/blob/main/Pictures/PCB.PNG)

The original Eagle design files are included as well as exported GERBER files for direct PCB production.

BOM:
- 1 x ESP32-WROOM-32 barebone
- 1 x 7 Pin SPI 0.96" Dual Color Yellow Blue OLED Display Module SSD1306 (https://hacktronics.co.in/lcd-displays/7-pin-spi-iic-096-dual-color-yellow-blue-oled-display-module-ssd1306)
- 1 x Mini USB female vertical TH (https://store.comet.bg/download-file.php?id=18384)
- 1 x MCP1826S-3302E/DB voltage regulator (https://store.comet.bg/download-file.php?id=4147)
- 3 x TANT B SMD 22uF 16V caps
- 2 x C1206 100nF 50V caps
- 2 x R1206 10K resistors
- 2 x R1206 4.7K resistors
- 1 x R1206 560R resistor

### Firmware
To upload the sketch you will need USB to serial UART converter capable of supplying 3.3V VCC.
Pinout for the header:
![](https://github.com/toto99303/Solo_DCF77_ESP32/blob/main/Pictures/pgm_header.png)

Remember that in order to boot the EPS32 in programming mode you will need to connect GPIO0 pin to GND (Low).

1. Open the sketch in Arduino IDE and edit your wifi SSID and password.
2. Use board "WEMOS LOLIN32" at 80Mhz flash frequency. (Tools -> Board)
3. Compile and upload.

### 3D printable stand

The original design file from Fusion360 is available as well as ready to print STLs.
![](https://github.com/toto99303/Solo_DCF77_ESP32/blob/main/Pictures/stand1.PNG)
![](https://github.com/toto99303/Solo_DCF77_ESP32/blob/main/Pictures/stand2.PNG)

### Video:

[![DCF77 transmitter - demo](https://img.youtube.com/vi/RjWDWWJ56to/0.jpg)](https://youtu.be/RjWDWWJ56to)

### More Pictures:

![](https://github.com/toto99303/Solo_DCF77_ESP32/blob/main/Pictures/ready2.jpg)
![](https://github.com/toto99303/Solo_DCF77_ESP32/blob/main/Pictures/pcb1.jpg)
![](https://github.com/toto99303/Solo_DCF77_ESP32/blob/main/Pictures/pcb2.jpg)



