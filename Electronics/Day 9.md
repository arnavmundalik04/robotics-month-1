Day 9 
Learning more about Arduino today. 
An Arduino comes with GPIO pins, pins that can be set up as either Input or Output pins. The pinMode function is used to do this. There are three types of modes that can be assigned.
1.	Input
2.	Output
3.	Input_Pullup
digitalWrite is used to write to a pin. It is usually used as an output for a component connected to a pin. Whereas digitalRead is used to read data from sensors attached to a pin. 
pinMode(pin number, direction);
digitalRead(pin number);
digitalWrite(pin number);

Making an arduino circuit with a push button. The configuration of the pushbutton is as shown. Both pins of group 1 and group 2 are always connected. 
For the LED + pushbutton circuit, we need a pull-down resistor. 
What happens WITHOUT the resistor?
This is the important part.
When the button is released, the Arduino input isn't connected to either 5V or GND.
It's floating.
A floating input can randomly read: HIGH, LOW, HIGH, LOW and so on. It is quite sensitive to noise. So, the resistor gives the input a default state: Button released: LOW
