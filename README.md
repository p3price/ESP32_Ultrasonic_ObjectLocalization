# ESP32_Ultrasonic_ObjectLocalization
- Simple example for ESP32 mcus and HC-SR04 Ultrasonic Sensors utilizing ESP-Now communication protocal.
- Three ESP32 are necessary for this example, two transmitters with ultrasonic sensors and one receiver connected to a pc via serial. (See the setup reference image)
- The two transmitting ESP32 read the ultrasonic sensor data and convert it to the distance that the reflecting object is from the sensor. The distance data is then transmitted to a receiving ESP32 that is connected to the host PC via the serial port. The receiving ESP32 concatenates the distance data and prints it as a x,y pair to the serial port. 
- The host pc is running a Touchdesigner project that reads the sensor data from the serial port and then plots the box on a grid. Visualization and audio cues show the user the position of the box in the grid and when it is centered on the grid. 

# Setup Reference Image

# Touchdesigner Network
<img width="1440" alt="Screenshot 2024-01-26 at 2 09 08 PM" src="https://github.com/p3price/ESP32_Ultrasonic_ObjectLocalization/assets/126983543/2425ae53-b865-4583-8d2c-0711997e7d6b">
