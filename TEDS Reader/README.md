This circuit was designed to read and write data on TEDS enabled devices such as microphones and accelerometers.
TEDS (Transducer Electronic Datasheet) is an IEEE standard for storing sensor information directly onto a small EEPROM chip using the OneWire protocol.
By supplying a constant negative voltage to the device, you are able to communicate with the internal memory.
The data saved in the TEDS architecture includes:
  Serial Number,
  Model Number,
  Manufacturer,
  Sensitivity,
  Calibration Date,
  and other relevant information relating to the sensor.
  
TEDS to OneWire Converter
  This page of the schematic describes a circuit that converts the negative TEDS signal to a positive OneWire signal. The OneWire protocol is easily readable using an Arduino and its corresponding library.
  It also contains a subcircuit which enables the internal TEDS chip to be written to as well.

-5V Generator
  This circuit uses a charge pump IC to take a 5V supply voltage from the Arduino and convert it to a -5V supply. It then gets regulated and limited to 2mA.

Arduino
  Anything interfacing with the Arduino is described in this section. 
  The Arduino is wired to an OLED using the SPI protocol and displays all relevant TEDS information.
  There are also two buttons. One signals to the Arduino to read the sensor and the other signals a write command to tag the sensor in the user data section of the memory.
