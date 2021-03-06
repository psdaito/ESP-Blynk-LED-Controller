# ESP-Blynk-LED-Controller

## Setup after programming ESP:

1. Check your available wifi networks for "LED AP" and connect to it, it should prompt you to select your wifi network and put in your Blynk token (best to copy it to your clipboard before running as there is a 5 minute timeout)
2. Once you've put in that info you should be able to connect via the Blynk app

## Once your Blynk app is connected:

1. Select Sunrise/Sunset, Daylight and Moonlight time period
2. Select "Fan On Temp", this is the temperature setpoint where the fan will be enabled when the heatsink reaches this temperature
3. Select Fade Duration, this is how long the app will take to ramp between light modes (if the ramp overlaps the next start time it will ramp from the current point to the new set values)
4. On setup tab select a test mode, ie "Test MaxPWM" which is your brightest mode
5. Move the sliders to the brightness you want
6. Hit the save button, this will save the current slider values to that mode
7. Repeat steps 4-6 for dim levels and moonlight levels
8. Set mode to normal operation and you should be good to go

## Hardware

### Breadboard wiring diagram:
![Breadboard wiring diagram](https://i.imgur.com/4xU6HxX.png)
Parts needed:
- Wemos D1 (or nodeMCU)
- DS18B20
- Adafruit PCA9685
- N-Channel MOSFet to drive fan

### Custom driver PCB
![Custom driver PCB](https://i.imgur.com/vgvPy1l.png)

## Libraries

- [Adafruit PWM Servo Driver](https://github.com/adafruit/Adafruit-PWM-Servo-Driver-Library)
- [Arduino JSON](https://arduinojson.org/doc/installation/)
- [Arduino OTA](https://github.com/esp8266/Arduino/tree/master/libraries/ArduinoOTA)
- [Blynk](https://github.com/blynkkk/blynk-library)
- [Dallas Temperature](https://github.com/milesburton/Arduino-Temperature-Control-Library)
- [Simple Timer](https://github.com/marcelloromani/Arduino-SimpleTimer/tree/master/SimpleTimer)
- [Time Library](https://github.com/PaulStoffregen/Time)
- [Wifi Manager](https://github.com/tzapu/WiFiManager)
