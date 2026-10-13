Day 11
A device which detects changes in electrical signals, chemical composition, physical properties and produces an electrical signal in response to that. Sensors can detect changes in temperature, level, flow, speed, position and pressure to name a few. A passive sensor needs external power to operate whereas an active sensor does not. 
Most sensors are connected to a transmitter because the sensors output needs to be conditioned or amplified. 
HC-SR04 Ultrasonic sensor
This ultrasonic sensor has 4 pins
1.	VCC: Connected to power supply, usually 5V. 
2.	Trig: This is the trigger pin. When you write HIGH to the trigger pin, it sends out a signal in the form of a square wave. 
HIGH           Then Low and slight delay            HIGH
Then the trig pin waits for the echo pin’s response. 
3.	Echo: After the trig pin gets triggered, the echo pin sets sends out a signal HIGH until it hears the trigger. So, the time for which the echo pin stays high is proportional to the distance of the object. 
A digital signal isn't always simply "ON" or "OFF." Sometimes you use a very short HIGH/LOW transition as a command or pulse. We do the digitalWrite low and then high because the TRIG pin needs a very short pulse to tell the ultrasonic sensor:
“Start a measurement now.”
It’s a signal. 
