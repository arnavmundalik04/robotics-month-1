Day 12
Watched the basis of a DC motor. 
This is the H bridge, by the way of the switches, we can complete the circuit and power the motor. 
For example, if Q1 and Q4 are closed, then the circuit is complete and the motors operates normally. However, if Q1 and Q4 are closed and then we close Q3, then it can cause a short circuit and bypass the route of the motor without ever powering it. 
Case 2: If Q2 and Q3 are closed, keeping Q1 and Q4 open, that also closes the circuit but the current flows in the opposite direction in this case. 
Remember NOT TO CONNECT THE MOTOR DIRECTLY TO THE ARDUINO. The Arduino cannot supply enough current that the motor demands. You need a motor controller for that. While making the circuit for this with multiple components like the Arduino, the motor driver and the power supply module, these components MUST HAVE A COMMON GROUND. 
Pin 1: EN1 controls the speed of the motor using PWM and analogWrite. 
Pin 2 and Pin 7: Controls the direction. If Pin 2 is high and 7 is low, the motor spins one way and vice-a-versa. 
Pin 3 and Pin 6 : These are connected to the motor. You connect both the wires of the motor to these. 
Pin 4 and Pin 5: These are ground pins. 

