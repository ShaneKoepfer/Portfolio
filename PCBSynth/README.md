This project is an attempt to make a single board synthesizer keyboard.
By changing the resistance on an oscillator IC, you can both set the frequency of a note and tune it using a potentiometer and resistor in series.
Each button is designated to a different resistance value which oscillates a buzzer at a set frequency.

Main Power  
  This circuit takes a 9V battery and converts and regulates the power to a 3.3V supply.

Frequency Generation  
  This page describes the oscillator, buzzer circuit, and resistances for each note. 
  There is also a circuit that changes the duty cycle of the oscillator using a potentiometer and op-amp.  

Button Multiplexer  
  This page describes the multiplexer and priority encoder circuit for the keyboard to prevent two buttons from being pressed at once.
  If each resistance was wired directly in parallel to the button, then it would be possible to press two buttons at once.
  If this were to occur, it would create an entirely new frequency outside of the tuned key. 
  This is due to the oscillator seeing a parallel resistance which would be equivalent to a smaller resistance than either of the two notes.  

  Thus, this circuit takes each button and routes them to two cascaded priority encoders.
  These ICs only allow one button to be pressed at once, preventing further issues when moving between notes.
  This then assigns each button to a binary value which is then routed to the multiplexer.
  Depending on the binary value going to the multiplexer, it routes a different resistance to the oscillator.
