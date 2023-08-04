# power-path-tasks
# task 1: LED matrix 
this is a code and simulation for an Arduino project that displays a 5x5 eye shape pattern on an LED matrix display.
Setup Instructions:
1. Go to [Tinkercad](https://www.tinkercad.com/) and create an account (if you don't have one already).
2. Create a new Arduino circuit in Tinkercad.
3. Drag and drop the required components onto the circuit workspace:
   - Arduino board
   - LED matrix display (5x5)
4. Connect the components as follows:
   - Connect the row pins (ROW_1 to ROW_5) of the LED matrix to pins 7 to 3 on the Arduino.
   - Connect the column pins (COL_1 to COL_5) of the LED matrix to analog pins A4 to A0 on the Arduino.
5. Open the Arduino code editor in Tinkercad.
6. Copy and paste the code from the led_matrix.ino file into the Arduino code editor.
7. Click on the "Start Simulation" button to run the simulation.

Usage:
1. The Tinkercad simulation will display a 5x5 eye shape pattern on the LED matrix display.
2. The pattern is defined in the eyePattern array in the code and represents the ON and OFF states of each LED in the matrix.
3. The code will iterate through each row of the matrix and activate the corresponding row pins (ROW_1 to ROW_5).
4. For each row, the code will set the column pins (COL_1 to COL_5) based on the pattern defined in the eyePattern array.
5. The eye pattern will be displayed on the LED matrix in the simulation.
6. # here is a tinkercad link: https://www.tinkercad.com/things/fzSVB0ka6Zq

--------------------------------------------------------------------------------------------------------------------------------------------------

   # electric circuit

this is a code and simulation for an Arduino project that controls an LED based on the state of a button. The LED turns on when the button is pressed and turns off when the button is not pressed.
 Setup Instructions:
1. Go to [Tinkercad](https://www.tinkercad.com/) and create an account (if you don't have one already).
2. Create a new Arduino circuit in Tinkercad.
3. Drag and drop the required components onto the circuit workspace:
   - Arduino board
   - LED
   - Push button
   - Resistors (if required for the LED and button)
4. Connect the components as follows:
   - Connect the anode (longer leg) of the LED to pin 7 on the Arduino.
   - Connect the cathode (shorter leg) of the LED to GND (ground) on the Arduino.
   - Connect one leg of the push button to pin 4 on the Arduino.
   - Connect the other leg of the push button to GND (ground) on the Arduino.
   - If necessary, add resistors in series to limit the current flow through the LED and button.
5. Open the Arduino code editor in Tinkercad.
6. Copy and paste the code from the button_led.ino file into the Arduino code editor.
7. Click on the "Start Simulation" button to run the simulation.

Usage:
1. The Tinkercad simulation will display an LED and a push button.
2. Initially, the LED will be turned on.
3. When the push button is pressed, the LED will turn on.
4. Releasing the push button will turn the LED back off.
# here is a tinkercad link: https://www.tinkercad.com/things/ibLfewLQoYv?sharecode=jYGpsJpUtha3RDbHEr2kfP-yOpPslKju3NY9UwiDS20

--------------------------------------------------------------------------------------------------------------------------------------------------

# task 2:
# servo motor 
this is a code and simulation for an Arduino project that controls a servo motor. The servo motor rotates from 0 to 180 degrees and then back to 0 degrees in a continuous loop. 
Setup Instructions:
1. Go to [Tinkercad](https://www.tinkercad.com/) and create an account (if you don't have one already).
2. Create a new Arduino circuit in Tinkercad.
3. Drag and drop the required components onto the circuit workspace:
   - Arduino board
   - Servo motor
4. Connect the components as follows:
   - Connect the signal wire (usually orange or yellow) of the servo motor to pin 9 on the Arduino.
   - Connect the power wire (usually red) of the servo motor to the 5V pin on the Arduino.
   - Connect the ground wire (usually brown or black) of the servo motor to the GND (ground) pin on the Arduino.
5. Open the Arduino code editor in Tinkercad.
6. Copy and paste the code from the servo_control.ino file into the Arduino code editor.
7. Click on the "Start Simulation" button to run the simulation.

Usage:
1. The Tinkercad simulation will display a servo motor.
2. The servo motor will rotate from 0 to 180 degrees in small increments, and then rotate back from 180 to 0 degrees in the same increments.
3. The rotation is achieved using the myservo.write() function, which sets the position of the servo motor based on the pos variable.
4. The for loops in the loop() function control the rotation of the servo motor by incrementing and decrementing the pos variable.
5. The delay(15) function is used to introduce a small delay between each position change, creating a smooth rotation effect.

Note: The servo motor is attached to pin 9 using the myservo.attach(9) function. Make sure to choose the appropriate pin based on your circuit setup.
# here is a tinkercad link: https://www.tinkercad.com/things/b15Gw36OjtJ?sharecode=kRw1s2ljX17nIntJJK1-y966tt6GISP6rQJXdMkp4ww

--------------------------------------------------------------------------------------------------------------------------------------------------

# DC motor 
this is a code and simulation for an Arduino project that controls a DC motor. The DC motor is driven by an H-bridge circuit, and the code enables the motor to move in a specific direction.

Setup Instructions:
1. Go to [Tinkercad](https://www.tinkercad.com/) and create an account (if you don't have one already).
2. Create a new Arduino circuit in Tinkercad.
3. Drag and drop the required components onto the circuit workspace:
   - Arduino board
   - DC motor
   - H-bridge module (L298N or similar)
4. Connect the components as follows:
   - Connect the enable pins (vA and vB) of the H-bridge module to PWM pins on the Arduino (e.g., vA to pin 3 and vB to pin 11).
   - Connect the input pins (i1, i2, i3, i4) of the H-bridge module to digital pins on the Arduino (e.g., i1 to pin 4, i2 to pin 5, i3 to pin 9, and i4 to pin 10).
   - Connect the power supply and ground pins of the H-bridge module to the appropriate power and ground connections on the Arduino.
   - Connect the DC motor to the output pins of the H-bridge module.
5. Open the Arduino code editor in Tinkercad.
6. Copy and paste the code from the dc_motor_control.ino file into the Arduino code editor.
7. Click on the "Start Simulation" button to run the simulation.

Usage:
1. The Tinkercad simulation will display a DC motor connected to an H-bridge module.
2. The DC motor will move in a specific direction based on the code in the move_DC() function.
3. The analogWrite() function is used to set the speed of the motor by providing a PWM value to the enable pins (vA and vB) of the H-bridge module.
4. The digitalWrite() function is used to control the input pins (i1, i2, i3, i4) of the H-bridge module, determining the direction of the motor rotation.
5. In the provided code, the motor is set to move in a specific direction by setting the appropriate input pin states. Adjust the pin states in the code to change the motor direction if needed.

Note: The specific pin assignments (vA, vB, i1, i2, i3, i4) in the code correspond to the hardware connections in the Tinkercad circuit. Make sure to adjust the pin assignments in the code based on your own circuit setup.

# here is a tinkercad link: https://www.tinkercad.com/things/39EYOwEnzhz?sharecode=BxOv-oi0xWU4Pn2SJKPz1f53dSEriC1KfgvZcnMgw1Y

--------------------------------------------------------------------------------------------------------------------------------------------------

# task 3:
# ultrasonic distance sensor
this is code and simulation for an Arduino project that utilizes an ultrasonic distance sensor to measure distances and control an output based on the measured distance. 

Tinkercad Simulation Setup Instructions:
1. Go to [Tinkercad](https://www.tinkercad.com/) and create an account (if you don't have one already).
2. Create a new Arduino circuit in Tinkercad.
3. Drag and drop the required components onto the circuit workspace:
   - Arduino board
   - Ultrasonic distance sensor
   - Output device (e.g., LED)
4. Connect the components as follows:
   - Connect the trigPin of the ultrasonic sensor to pin 9 on the Arduino.
   - Connect the echoPin of the ultrasonic sensor to pin 10 on the Arduino.
   - Connect the output pin (e.g., pin 8) to the input of the output device (e.g., LED).
5. Open the Arduino code editor in Tinkercad.
6. Copy and paste the code from the distance_sensor.ino file into the Arduino code editor.
7. Click on the "Start Simulation" button to run the simulation.

Usage:
1. The Tinkercad simulation will display the distance between the ultrasonic sensor and an object in centimeters.
2. If the distance is equal to or less than 50 centimeters, the output device (e.g., LED) in the simulation will be turned on. Otherwise, it will be turned off.

# here is a tinkercad link: https://www.tinkercad.com/things/huMuRpiJjaE?sharecode=8Idri3553TtCFNYwj21MClgtQCbhk6y99KoE0mik068
