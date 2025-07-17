# Flysky Arduino
Flysky FS-i6X Integration with Arduino

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
- The switch SWA will give values of 0 or 1, depending on its position. Everything else will range between -100 and 100, with zero being the center.

## REFERENCES

- [DroneBot Workshop Tutorial](https://dronebotworkshop.com/radio-control-arduino-car)
- [How to Set Up Flysky FS-i6X AUX Switches](https://github.com/bmellink/IBusBM)
- [Arduino iBusBM Library](https://github.com/bmellink/IBusBM)
