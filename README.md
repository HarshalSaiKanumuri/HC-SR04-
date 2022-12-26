# HC-SR04 to Measure Range

The HC-SRO4 is an Ultrasonic ranging module which is said to provide reliable readings between 2cm to 4m of an object. " The ranging,accuracy can reach to 3mm "
, which means that data + or - 3mm from the true value. The HC-SRO4 sensor sends 8 cycles of 40KHz ultrasonic waves when a 10us high signal is send to the trigger.
If some ultrasonic waves are successful in reflecting on the intented object , the time between the sending the signal and reciving the signal can be calculated.
Using ( Velocity of Ultrasonic waves ) * ( time taken by ultrasonic waves to be reflected back / 2 ) = Range of the object.
All this information is available in the HC-SR04 data sheet : https://cdn.sparkfun.com/datasheets/Sensors/Proximity/HCSR04.pdf

Below is the wiring of the HC-SRO4 for Aduino:

![image](https://user-images.githubusercontent.com/121031084/209546791-98dfa85d-782b-40a6-94f8-6973a59b86f0.png)

Below is the wiring of the HC-SRO4 for ESP-32:
( Important note : The echo pin on the HC-SR04 sends a 5V signal to GPIO pin used , this will damage the pin. Hence this voltage is divided so 3.3 V is sent ) 

