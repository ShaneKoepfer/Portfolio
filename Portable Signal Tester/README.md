This device was intended to be a portable solution to help troubleshoot data acquisition systems. 
The circuit acts as a Low Frequency Oscillator (LFO) that generates a square wave signal at 1Hz that is then converted to a voltage and current controlled sine wave. 
These signals are then passed through a series of op-amps that amplify at different amplitudes that are common for most acquisition systems.   
The signals generated include:  
+/-2.5V Square  
+/-12V Square  
0-24V Square  
+/-50mV Sine  
+/-1V Sine  
+/-5V Sine  
+/-10V Sine  
+/-20V Sine  
0-1V Sine  
0-5V Sine  
0-10V Sine  
4-20mA Sine  

Dual-Rail Power Supply  
The back side of the PCB contains the power supply circuit. The device takes two 9V batteries and boosts the voltage to 24V. 
This works due to the circuit being relatively low power as it does not need much current to generate the oscillating signal.

1Hz Voltage Function Generator  
This is where the LFO is detailed and describes the +/-2.5V square wave generator and the +/-1V sine wave generator. 
Each subsequent op-amp circuit either boosts or bucks the amplitude of the oscillator circuit to the desired voltage.

1Hz Current Function Generator  
This circuit depicts the conversion circuit from the 0-5V sine wave circuit to the 4-20mA sine wave signal. 
The rotary dial switch is also described here, showing the switching between each signal being passed to the analog output.
