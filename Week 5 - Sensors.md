---
title: Week 5 - Sensors
tags: [CART 360]
created: 2024-10-03T22:54:30.469Z
modified: 2024-10-03T23:24:19.814Z
---

# Week 5 - Sensors

Voltage division 

Vout = R2 / (R1 + R2) = Vin

This is what's used for most sensors

Every sensor creates an *analog output*, sometimes directly connected to an output pin, or processed internally in order to create a binary or digital input

Photoresistor ex.
photon lands, if there's photons there, resistance changes, we see the difference directly

## Sensor domains:
Analog output
- Voltage
	- Not changing the info, just looking at voltage
- resistance
	- ex: thermistor (resistance changes because of heat), photocell 
- Open collector
- Current (not for us)

From analog,
Binary
- high/low
	- ex. buttons!
	- either on or off
- PWM
	- pulse width modulation
	- making things look like in betweens
- Frequency (not for us)
Digital
- microcontroller creates a digital discretization of external world for us to work with
- 2 types
	- I2C
	- SPI

*When talking about voltage, we can reason and rationalize how we interpret it*
We can move away from physical impetus or return to it as we please

### Analog sensor
ANalog voltage output can be connected directly to an analog input, so long as range is compatible and sensor can provide sufficient current

voltage goes from sensor, through two resistors, with reduced voltage output in between them
voltage division!!!

Variation:
sensor could also be one of the resistors

### Open-collector
When sensor is triggered, current is diverted from microcontroller to sensor
So high means no sensing, low means yes sensing

### Binary
A sensor that provides a binary output can be connected directly with a microcontroller if voltage range is variable
(a button could have an led that requires more voltage than the microcontroller can handle, thus causing you to have to protect it)

#### PWM
emits fixed frequency, but variation of width

### Digital
A bus is a communal pathway for sharing data among components or devices

Microcontroller Utilises UART (a serial protocol), the voltages of which are then translated into USB territory

bits per second is also pulses per second
These then pass through the bus

Bus is in parallel...

You can't expand I/O, General pins
Choosing which serial communication is important!

UART - 3 wires
I2C - 3 wires
SPI - 5 wires (faster, but!)

### voltage dividers
A voltage divider involves applying a voltage source across a series of two resistors. 
