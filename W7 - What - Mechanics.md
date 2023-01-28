---
title: W7 - What - Mechanics
title_custom: true
tags: [Intro to Game Design]
created: 2022-11-27T21:01:56.243Z
modified: 2022-11-27T22:10:12.461Z
---

# What are games made out of?

**Mechanics** <-> Dynamics <-> Aesthetics

This is the stuff we can actually design

## Mechanics, sliced

Interface --- The means through which players interact with everything
    ^
 Systems --- Bundles of mechanics that interact in dynamic ways
    ^
Mechanics --- Recognizable and generalizable bundles of rules (ex. taking cover)
    ^
  Rules --- What players can do, can't do, have to do, fiddle with
  
Ex.

Navigation system
       ^
Moving, jumping, running, fast travel, minimap
  ^
button pressed = 1 unit in one direction
_________________

Combat system
      ^
blocking, punching, hp managaement, aiming, weapon switching
                                                   ^
       nb of weapons: max 5, tab key cycles through

## Rules
The minimum requirement for a game to exist

Ex. Yes or No
Rule: Answer questions as long as possible without saying "yes" or "no"

### Explicit rules
Rules that are clearly defined and known to all players

Ex. Monopoly
Throuw the dice and move token approp. amount of spaces

### Implicit rules
Unwritten, expected behaviour, "etiquette"
Ex. Move the token in a timely fashion, once something is down it's played don't take it back

### Game materials
Materials and equipment, state of the world, are part of the rules

Ex. Monopoly: board dictates what the spaces are you can move in
Ex. bindeogame: you stop moving when you bump into an object, location of objects is part of the rules
Ex. Yes or No: humans are required material

Can be very strictly defined: specifications for sports equipment

If an element in the map in a multiplayer game is only present for one player,
they are not playing the same game
Even colour can matter!

Rule of thumb: if it's in the game, it's a rule

Materials in games:
- Visuals
- Narratives
- Levels
- Layouts
- Etc.
-> Content

### Goals
A special kind of rule
What the players are trying to achieve (within constraints of rules)
Goals carry some intrinsic motivation

Ex. Yes or No: talk as long as possible

Why?
Gives meaning and direction for play

Salen & Zimmerman:
Goal is at center of magic circle, pole that holds tent (game) aloft, players are inside the tent, playing with one another, the goal sustains tent, interest, engagement, desire

Types of goals:
- Narrative
- Formal

## Mechanics (Mechanisms)

Ex. Yes or No
Rule: can't say yes or no
Goal: Answer as many questions as possible
Materials: mouths and ears

Mechanic: Word avoidance

Fuzzy concept
Building block of design
Higher-level notion than rule
bundles of rules working together in a meaningful way
Synonyms:
- Game atom
- Ludeme
- Game patterns

Examples:
- Trump cards
- Bidding
- Double-jumping
- Shooting
- Action queueing 
- Turns
- etc.

### Abstractions
Operate according to specific rules in diff. games
Can thus be implemented differently in different games
Bidding in poker: Money on the table
Bidding in bridge: calling number of tricks to be made

### Repertoire
Mechanics represent a designer's repertoire
Mechanics have a history: they can be traed to an original game
Innovation often comes from new combinations of existing mechanics

## Language metaphor
Game pieces, objects = nouns, inventory, gun, crate, objects
Game actions = verbs, we've used that for mechanics
Rules = grammar, describe how nouns and verbs can be put together

Ex. Mario
Jump! Collect! - verbs
Coin, Platform, power-up, - nouns

## Reminder:
Mechanics are ultimately defined as rules
Jumping mechanic
When player presses a, avatar has an upward force momentum of 10

## Systems
Systems allow us to see the interconnectedness between stuff in games

One can graph the connections between systems
Analyse how relevant elements or systems are, how important are they?
Systems can have subsystems, increase complexity

Thinking in systems: Monopoly
1. p1 initial **state**: 1500$, 0 properties, 0 buildings
2. Lands on Kentucky. Decides to buy (**interaction**)
3. P1 updated **state**: 1280$, 1 property, o buildings

Kentucky also has properties, ie. colour and value

Systems designer is a job!

Systems are most useful as a lens through which to analyse dynamics over time

Will talk about it later

## Interface
player  <->  input & feedback  <->  game
                Interface!
                
**Inputs**
The measn through which a player communicates their intention of action to a game
- Pressing buttons
- Moving joysticks
- moving a token
- etc.

Often, what everyone else chooses makes most sense

**Feedback**
How a game communicates changes in game states to players
- Avatar movement
- Revealing a card
- Moving the camera
- Particle effects
- etc.

Often, interface design aims to make things efficient, transparent
Not necessarily so in games
Ex. 1st person shooters
Predicated on the idea that one's view is severely restricted by the perspective
Dead Space: Isaac is slowww

### The 3 Cs: Character, Controls, Camera
Input and feedback are mainly communicated via above
How these work can sum up how a game feels

Mario Kart 7:
First person mode, 3D, gyro controls

Dead by Daylight:
1st person for killers, 3d person for survivors

### Problem in games
There is often no distinction between interface and the "game" as an abstraction
Designing the world inherently involves designing feedback in game world
One has to be aware of game looks

Ex. Blue crates in a shooter: blue colour makes them stand out, invites you to interact with them

### Affordance and Constraint
**Affordance**
"Perceived and actual properties of the thing, primarily those fundamental properties that determine just how the thing could possibly be used"
An encouragement for a certain type of action

**Constraint**
"Powerful clues, limiting the set of possible actions, in order to let people readily determine the proper course of action, even in a novel situation"
A limitation to certain types of actions

A door with a handle affords pulling, although it can still be pushed
A door with only a plaque constrains pulling and affords pushing

Quotes from Don Norman, *The Design of Everyday Things*

Clicker games
Pure system
Pure interface
