# Arduino-DOOM
DOOM running on an Arduino UNO R3 + 0.96" OLED + 5 Buttons + Buzzer

"it runs DOOM" - on 2KB of RAM

### **Specs**
- **Board**: Arduino UNO R3 
- **Display**: 0.96" SSD1306 OLED 128x64 I2C
- **Controls**: 5x Push Buttons - D-Pad + Fire
- **Audio**: Passive Buzzer for SFX
- **FPS**: ~4-8 FPS

### **Wiring**
| Component | Arduino Pin |
| --- | --- |
| **OLED GND** | GND |
| **OLED VCC** | 5V |
| **OLED SDA** | A4 |
| **OLED SCL** | A5 |
| **Button Up** | D2 |
| **Button Down** | D3 |
| **Button Left** | D4 |
| **Button Right** | D5 |
| **Button FIRE** | D6 |
| **Buzzer +** | D9 |
| **Buzzer -** | GND |

All buttons use `INPUT_PULLUP`. One side to 5V, other side to pin.

### **Controls**
`D2-D5` = Move / Look  
`D6` = FIRE / Open Door

### **Libraries Needed**
1. `Adafruit GFX Library`
2. `Adafruit SSD1306`

### **Build Notes**
The UNO is at ~95% RAM usage. Code uses PROGMEM for maps/textures. 
Sound effects are generated with `tone()` on pin 9.

### **Credits**
Find my other projects from: https://sites.google.com/view/codeandcirkit?usp=sharing

Built by: Thiyon(Code&Cirkit)
