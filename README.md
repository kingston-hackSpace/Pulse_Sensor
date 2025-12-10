# Pulse Oximeter & Heart Rate Sensor

The ***Pulse Oximeter & Heart Rate Sensor*** is made of two chips (MAX30101 & MAX32664 ). Together, they perform biometric sensing.  

The *MAX30101* gets your heart rate (BPM) and blood oxygen levels (SpO2) through the process of photoplethysmography (obtaining biometric data with light).

The *MAX32664* receives the data and runs the calculations to determine heart rate and blood oxygen.

### HOW DOES IT WORK?

When placing your finger gently on the sensor (which shines red/infrared light through your skin), the capillaries filled with blood under your skin will absorb this light or not, and the MAX30101 sensor will read which light comes back. This light data will then be sent back to the MAX32664 which handles all the calculations to determine heart rate and blood oxygen levels.

### MORE INFO

Read more about the Pulse Oximeter & Heart Rate Sensor [here](https://learn.sparkfun.com/tutorials/sparkfun-pulse-oximeter-and-heart-rate-monitor-hookup-guide)

----
# TUTORIAL
----
### HARDWARE

- Arduino UNO
- Pulse Oximeter & Heart Rate Sensor

----
### WIRING

⚡ Warning! Remember, this biometric sensor supports **3.3V only**. 

SENSOR | Arduino
-|-
SCL | SCL
SDA |SDA
3V3 | 3V3
GND | GND

----
### CODE AND INSTRUCTIONS

- Download the corresponding libraries [SparkFun_Bio_Sensor_Hub_Library](https://github.com/CamilaColussi-KSA/SparkFun_Bio_Sensor_Hub_Library)

- Install the libraries via "Importing a .zip Library". Instructions [here](https://docs.arduino.cc/software/ide-v1/tutorials/installing-libraries/)

- Open Arduino IDE and find the sensor examples:

    - File > Examples > Adafruit TCS34725 > tcs34725

- Upload the code to your Arduino board.

- Open Arduino's Serial Monitor to see the incoming data.
