Link to our research paper: https://docs.google.com/document/d/1riK_md2-noeCT2EpTjOqRZSLSGz6CT_NuyUZCUM05jI/edit?usp=sharing


Materials list:
- acryllic sheet
- 3d print filament (white and gray)
- two big servo motors (MG996R Servo Motor)
- two small servo motors (SG90 Micro Servo Motor)
- brush that will scrub the underwear
- M2.5 screws, M3 screws
- water pump
- silicone tubing that fits water pump
- relay
- arduino
- 2 power supplies (5V, 10A & 5V 4A)
- power cable for arduino


To get started, 3D print the robot-arm parts, the sink, the faucet and the brush-holder part. You can find all the 3D printing files in the "Building the Project" - "3d print" folder. 

We followed this tutorial to assemble the robotic arm: https://howtomechatronics.com/tutorials/arduino/diy-arduino-robot-arm-with-smartphone-control/

Next, laser cut the ground plate using the prepared laser cut file in the "Building the Project" folder. 
After cutting out the plate, position the sink, Arduino, relay as well as the robotic arm on the desired position,and mark the mounting holes with a permanent marker. 
Carefully use a drill to drill the correct size hole through the ground plate. Don't forget to drill an extra hole for the wires of the servo motors. 
Mount all parts using the M2.5 screws. 

Wiring: 
Next, connect all positives of the motors of the robotic arm as well as the negative ones into two big bundles, solder them to a thicker wire and connect them to your 5V 10A power source. Connect the GND of the power source to the GND of the Arduino. Then, connect the data pins of the servo motors to the correct pins of the Arduino. To wire the relay, connect the relay to power, ground and data using pins from the Arduino on one side of the relay. On the other side, connect one pin to the 5V of the water pump, and the other side to the positive end of your 5V 4A power source. Then connect the GND of the power source to the GND of the water pump. 

Upload Arduino Code:
Next, upload the Arduino code provided in the  "Building the Project" folder to your arduino. 
Close the serial monitor of the Arduino IDE, and start your node application. Double check that the port name in the code of the app.js file is the same as the port to which your Ardunio is connected. 

Test:
Go to your n-point endpoint and change 0 testday times to your current time. If everything works correctly, the water pump should first start pumping water for 5 seconds. After that, the robot arm should start sweeping.


