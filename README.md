# Flysky-Arduino
Flysky (FS-i6X + FS-iA6B) Integration with Arduino

| ![image](Flysky%20FS-i6X.jpg) | ![image](Flysky%20FS-iA6B.jpg) | ![image](Arduino%20UNO%20R3.jpg) |
|:-----------------------------:|:------------------------------:|:--------------------------------:|
| **Flysky FS-i6X**             | **Flysky FS-iA6B**             | **Arduino UNO R3**               |

## SETUP

- **Transmitter:** [Flysky FS-i6X](https://www.flysky-cn.com/i6x-gaishu-1)
- **Receiver:** [Flysky FS-iA6B](https://www.flysky-cn.com/ia6b-canshu)
- **Controller:** [Arduino UNO R3](https://docs.arduino.cc/hardware/uno-rev3)
- **Connections:**

  | Arduino* | FS-iA6B |
  |----------|---------|
  | GND      | GND     |
  | 5V       | VCC     |
  | 3        | 1       |
  | 5        | 2       |
  | 6        | 3       |
  | 9        | 4       |
  | 10       | 5       |
  | 11       | 6       |

  *Use PWM Pins on Arduino

## USAGE

- Disconnect the Arduino from the computer while you power up the transmitter.
- Connect the Arduino and open your Serial Monitor. You should start seeing a display of all six channels.
- Manipulate the remote controls and observe the Serial Monitor data. You should see that each control affects a specific channel of data.
- CH6 (switch SWA) will give boolean values of 0 or 1, depending on its position. Everything else will range between -100 and 100, with zero being the center.

## REFERENCES

- [DroneBot Workshop Tutorial](https://dronebotworkshop.com/radio-control-arduino-car)
- [How to Set Up Flysky FS-i6X AUX Switches](https://github.com/bmellink/IBusBM)
- [Arduino iBusBM Library](https://github.com/bmellink/IBusBM)
