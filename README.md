#Auto Water

The initial goal of Auto Water is to automate watering of plants utilizing moisture sensors and ultrasonic sensors.

#Current State

Currently, you can only turn the pump on and off, I do this remotely from my desktop into the Pi and run my script for testing.

#Next Goal

Adding of a breadboard to process the analog output from the current moisture sensor I'm using

#Further Goal

Adding of a web interface to manage and track data of the plants

#Final Goal

Extending and scaling up the amount of plants to turn this into more of an automated irrigation system based on the needs of the plants

#Materials needed
You will need the following materials to replicate this:
1. Raspberry Pi 3/4, I'm currently using the Pi 4 Model B
https://www.pishop.co.za/store/index.php?rt=product/product&product_id=1729

2. Mini micro submersible pump, roughly 5v power required
https://reliablestore.co.za/products/mini-micro-submersible-motor-pump-water-pumps-dc-3-6v-100l-h-low

3. USB cable to strip for a power source

4. Dupont/jumper cables for connections
https://www.robotics.org.za/RIB-COMBO-10?search=ribbon%20cable%20combo%20m-m%2C%20m-f%2C%20f-f%2010cm

5. Moisture sensor
https://www.takealot.com/gravity-analog-capacitive-soil-moisture-sensor-corrosion-resista/PLID56355682

6. 5V Relay
https://www.robotics.org.za/index.php?route=product/search&search=4%20Channel%20Relay%20Module%20-%20Opto-Isolated

With regards to the moisture sensor, if you utilize the same as I have, you will require a breadboard/ADC Converter in the future for automation as it does not have a digital output. I would recommend this as an ADC Converter https://www.dfrobot.com/product-1730.html

#Setup

You will need to have a version of python 3 installed and once that is done, you will need to get setup for RPIo

This command should do the trick:
python3.4 -m pip install RPi.GPIO

At this point, you should be able to run the script like this:
>python3
>>> import water
>>> water.pump_on()

Provided you're all wired up, that should work.
