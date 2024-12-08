---
title: Week 8ʔʔ - Loads
tags: [CART 360]
created: 2024-11-07T23:26:23.605Z
modified: 2024-11-08T00:10:17.460Z
---

# Week 8ʔʔ - Loads

What do you do when a motor you want to use requires more voltage / amperage than you can provide?

Or you want to use AC powered lights / motors / home things

These are all **electrical loads**

If a component in a circuit is doing meaningful work, it is **loaded**

Elio ex.
Blender controlled by a microcontroller
Orchestra of kitchen appliances turned on and off by a microcontroller

#### Transformers or transistors
Generally, we'll stay with transistors

we can interface low voltage with high voltage

## Transistors
Basis of modern electronics
We'll focus on a specific use, controlling high power circuits with a low power microcontroller

Transistors allow you to generate a signal while protecting ur microcontroller

### pnp and npn
plates with canyons ( for an electron) between, we get electrons to jump across
Difference between them is direction of the emitter
pnp expects something going into it, npn expects something to pass through it

### Types

#### BJT
transistors are controlled with current going into base
you have to be careful not to overflow it
dont wanna peak, wanna control it slowly, with resistor

transistor modulates current going to another device

if u pwm 50% into the base, transistor will pass 50% of the external power source

Have BCE Base control emitter

#### FET
Field effect transistors (MOSFETS)
really really fast,
useful for audio, radio

BJTs will saturate if you pulse too fast

Gate (= base) Drain (= control) Source, common ground (= emitter)

signal goes down to gate, pulldown resistor to ground
sensitive to voltage instead of current

## Motors
Many!!!!

### Types

#### Brushed
Contact inside
bit of electrical noise
speed limitation due to brush heating, melting, arcing
could cause microcontroller to reset because of noise, would have to work on circuit to isolat

#### Brushless
no contacts!
no electromagnetic feedback
difficult to control

#### Steppers (geared)
Very position accurate!
Require a lot of current, constant
step size limit speeds
ex. step size is 3.6 degrees, 100 steps, brusque

#### Assemblies
cheap brushed
Use gears for torque
cheap, but torquey
gears on cheaper ones made from nylon, will wear out easily from strain, blocking
go with more expensive metal ones!
or cheap ones won't sit correctly, will skip, jitter, etc.
gears could be too loose or too tight

#### servo motors
simple to control
limited range of motion, 180 (RC)
or continuous motion
cheaper ones, analogue driven (potentiometer)
in this case, will drift more as it warms up, flow is better
this is not a problem with optically encoded servo motor

Stalling motors are bad!!!!
Will sink increasingly more current to overcome
If it can't, could melt wires!

### power

they are power hungry!!!
not well behaved loads!

### don't
over
under
voltage a motor, will damage
(if it's expensive)

### protect
thicker wires are better!
Can withstand higher amperage for longer (16 or 20 gague for 5 amps) before melting

### movement
circumference is important!!!
can allow us to know how many revolutions we need for a given amount of linear movement
