Day 4
Power: P = V x I
Where V = voltage is the specific work (or potential energy) per unit charge.
I = Current, it is the rate at which electric charges move through a conductor. 
Voltage (specific work) is analogous to the work done in lifting a weight against the pull of gravity. Current (rate) is analogous to the speed at which that weight is lifted. Together as a product (multiplication), voltage (work) and current (rate) constitute power. Whether we measure power in the unit of ”horsepower” or the unit of ”watt,” we’re still talking about the same thing: how much work can be done in a given amount of time.
When a motor is connected to a power supply, the motor decides or draws the current it needs to. The battery doesn't simply “push its maximum current” into the motor. The motor draws the current its electrical/mechanical conditions demand, within the limits of the battery, wiring, driver, etc.
Motors can be electrically difficult because they can demand a lot of current when starting or when they are overloaded. 
While powering a motor, 
Arduino → [BASE RESISTOR] → Transistor
↑
limits current
You want a flyback diode across the motor for that inductive spike, so the motor is not damaged if electricity is switched off. 
       +V
        │
      MOTOR
        │
        ├─────────┐
        │         │
        │        diode
        │         │
     transistor───┘
        │
       GND


Arduino GPIO
     ↓
small control current
     ↓
transistor
     ↓
large motor current
As the motor spins, it generates a voltage that opposes the battery voltage. This is called back EMF (back electromotive force). 
I=  (V-Vback)/R	

When the motor starts, current can be huge. But when it starts spinning, back EMF increases and the current falls. 
More mechanical load → motor slows down → less back EMF → more current drawn by motor.
If the motor stall, very high current. Higher current heats the motor up more. 
