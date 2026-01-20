# Pulse Sensor Amp

Reference image [here](https://github.com/kingston-hackSpace/Pulse_Sensor/blob/main/PulseSensor_1.webp)


Watch video: [Pulse Sensor](https://www.youtube.com/watch?v=RbB8NSRa5X4)

Read more: [Compatible micro-controllers](https://pulsesensor.com/products/pulse-sensor-amped)

Read more: [About Pulse Sensor](https://pulsesensor.com/products/pulse-sensor-amped)

----
## HOW IT WORKS

The sensor is essentially a small optical heart rate monitor that uses photoplethysmography (PPG). An LED shines light into your skin, and a light sensor measures how much light is reflected back. As blood pulses through your capillaries with each heartbeat, the amount of reflected light changes. These tiny changes create a waveform that corresponds to your pulse.

- The sensor relies on steady contact between the LED, the skin, and the light sensor.

- If the finger moves, lifts slightly, or presses unevenly, the reflected light drops.

- Shield the sensor from bright ambient light where possible.

----
# TUTORIAL
----
## HARWARE

- Arduino UNO

- LED + 20ohms resistor (x2)
  
- Pulse Sensor KIT:

  - Pulse Sensor
  
  - Premium Braided Cable

  - Ear Clip (for alternate placement options)

  - Velcro Finger Strap (for secure attachment)

  - Transparent Vinyl Dots (for electrical insulation)

----
## WIRING

The PulseSensor comes with a 3-cable ribbon cable terminating in a male header. The pinout is as follows:

Purple Wire = Analog Pulse Signal

Red Wire = Vdd, Power with 3V or 5V

Black Wire = Ground

More about wiring in the tutorial below

----
## CODE and INSTRUCTIONS

- Open the Arduino IDE and install the "PulseSensor Playground":

    - Open your Library Manager
 
    - Search for "PulseSensor Playground" and install
  
- Please follow the next two tutorials in the order provided.  

STEP 1: [Analog Signals tutorial](https://pulsesensor.com/pages/code-and-guide). This code was designed to visualise analog signals from the sensor by using the Arduino Serial Plotter. More stable signals for further visualisations will be explored next. 

STEP 2: [BPM](https://pulsesensor.com/pages/getting-advanced), you will find 2 tutorials:

          - Getting BPM to Monitor: get BPM data and print it to the serial monitor.
          
          - Pulse Sensor BPM : turn on an LED based on Heart Beats. In your code, the variable "pulseSensor.outputSample()" prints 3 data types:

                1. BPM (Beats Per Minute).
                
                2. The raw analog signal from the Pulse Sensor.
                
                3. An smoothed or processed signal.

Now you understand the sensor's outcoming data, you can use it for more advanced projects:

[Processing Heart Beat Visualiser](https://github.com/WorldFamousElectronics/PulseSensor_Amped_Processing_Visualizer)

[Pulse Sensor Speaker Tutorial](https://pulsesensor.com/pages/pulse-sensor-speaker-tutorial)

[Pulse Sensor Servo Tutorial](https://pulsesensor.com/pages/pulse-sensor-servo-tutorial)

For more tutorials, explore Arduino and Processing at the [left side menu of this page](https://pulsesensor.com/)

----
## SET UP ADVICE

Squeezing the Pulse Sensor too hard against your skin will make the heartbeat go away, and not enough pressure will cause too much noise. 

If the code is reading too many Beats Per Minute, or you are getting lots of noise, try adjusting the Threshold setting. The Threshold variable tells Arduino when to find a pulse that is legit. Adjust the Threshold value (noted above with arrows).  The Threshold can be any number between 0-1024, but try adjusting by steps of 5 or 10.  Decreasing the Threshold increases the sensitivity.  Increasing the Threshold decreases the sensitivity.  
See if you can find a better threshold for your finger than our default value.



----
## 3D PRINT

The PulseSensor is incredibly sensitive, which is usually a good thing. But sometimes, it's a bit too sensitive. A minor movement can mess with the data readings. 

The [Stabilizer Ring](https://pulsesensor.com/products/gold-stablizer-ring) (available for 3D printing) enhances user comfort for both short-term and long-term readings. It also expands a user's freedom of movement while wearing the sensor.

Download 3D file (stl) [here](https://github.com/kingston-hackSpace/Pulse_Sensor/blob/main/PulseSensorStabilizerRing.stl)
