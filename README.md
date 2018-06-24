# MFRC522 i2c 
### Code is compatible to Arduino and ESP8266 (NodeMCU)

1. [Download and install following library from arozcan](https://github.com/semaf/MFRC522-I2C-Library)

2. __Set the Pin for the RST and i2c address!__
```c++
#define RST_PIN 6 // Arduino UNO
// #define RST_PIN 14 // D5 on NodeMCU

// 0x28 is i2c address of the NFC Reader. Check your address with i2cscanner if not match.
MFRC522 mfrc522(0x28, RST_PIN);   // Create MFRC522 instance.
```