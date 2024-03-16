---
title: W8 - What - Dynamics
title_custom: true
tags: [CART 215 - Intro to Game Design]
created: 2022-11-27T21:01:56.243Z
modified: 2024-03-15T18:36:32.059Z
---

# What Are Games Made Out Of?

## Activity
We don't buy a fan for the plastic and wiring that makes it up, but rather for the activity it does, the wind it produces

We are not designing dynamics directly

Mechanics -> **Dynamics** -> Aesthetics

## EX: 
Dynamics in soccer:
- Running on the field
- Passing
- Interrupting a pass
- Stealing the ball
- Shooting at the goal
- Blocking the shot

These are not specified by the rules of the game (mechanics)
They arise from players trying to achieve goals, while constrained by rules

Running in soccer
- One has to bring ball to gal
- Enemy wants to take it to the other goal
- I need to get to the ball first
- I need to *run*

Assorted
- Poker - Bluffing
Shooters - Taking cover
Tennis - smashing, lobbing


## Metaphors
Language
Mechanics = nouns, verbs, grammar
Dynamics = What players *say* with the mechanics
Conversations thus emerge from what players say

Mechanics are tools, dynamics are what is done with the tools

## Loops
Repeated       **HEYO, NOT FINISHED**
A tool to understand and plan player activity

### Frequencies
- **Micro Loops**: short frequency, motivated by short term-goals
Run, get the ball, pass the ball, receive a pass, etc.
- **Macro Loops**: Longer frequency, motivated by long-term goal
Gain ground, losing ground, obtaining oppportunities to shoot at goal

### TimeLoop Diagram
Imagine progressively bigger circles around loop elements

Ex:
Monopoly
Bankrupt other players           -> 60 minutes
Complete sets                    -> 20 minutes
Buy property, Buy hotels         -> 5 minutes
Move on board, get/lose money    -> 1 minute

Diablo
Experience the story
Progress through levels, skill trees, etc.
Venture, fight, return, sell & trade
Kill and loot

The Sims
Manage a neighbourhood
Advance at work, build friendships, have a family
Go to work, make money, socialize,
Eat, poop, sleep

### Core Loop
'"Minimum viable" level of activity: the smallest kind of a loop that's going to be meaningful and enjoyable to the player and give them a reason to keep playing'

EX:
- For Diablo, venturing, fighting, returning, selling & trading
- For The Sims, going to work, making money, socializing

Core loop gives a sense of priority, what is most important and compelling, how can rest of design support and emphasize the core loop?

Could be compared with the idea of a game atom, how long is it? Where does it fit? How does this impact pacing and feel?

### Considering player motivation in loops SLIDES
Why would a player do it?
Is it about challenges?
Story?
Aesthetic?
Is your game falling flat? Is the core loop working?

### Types of loop
- Challenge loop
... Objective
- Curiosity loop
... Question -> Hypothesis -> Satisfaction ...
- Sensorial loop
... A new sensory proposition -> Exploration -> Habituation ...
Ooh, a new type of area! What's in it? Ok, I've seen it, I'm satisfied
- Social loop
... Interaction opportunity -> Leveraging that opportunity -> Player reaction ...
Ooh, can I hide that I'm an impostor successfully? A-ha! A moment to blame another player! Yes, they all thought I was a crew member

### Rewards 
Tool to turn loop wheel
- Help shape behaviour by incentivising or not certain actions
- Currencies , items, abilities, story progress, unlocked space, achievement, etc.

Need to be **valuable** 
XP and Gold are worthless in themselves, but, 
- XP -> Levels -> Power -> more XP!
- Gold -> New items -> Power -> More gold, more XP!
Anecdote: in a semester of only clicker games, the most compelling one was the most stingy game, making him want to acquire clicks as much as possible

**Reward schedules**
Ref: behaviourism, operant conditioning
- Continuous: each action
The moment you stop giving, players lose interest
- Fixed interval: each C seconds
- Fixed ratio: each C actions
- Variable interval: each x seconds
- Variable ratio: each n actions

RPG example
Why should a player attack monsters?
- Killing a monster always gives u XP + items (**continuous reward**)
- Sometimes, the loot is much better than others (**Variable interval**)
- Once you reach enough XP, you level up (**fixed ratio**)

### Progression
Considering player engagement on the long run, how to keep game loops fresh?
EX:
- Climbing the skill ladder (rankings, better opponents)
- Unraveling intricate story
- Beating all the levels
- Unlocking new content
- Becoming a mentor
- Increasing difficulty
- Trying again, differently (new character, mode, difficulty)
Etc.

## System dynamics

System ex: Monopoly
- P1 initial stateL 1500$, 0 properties
- Lands on Kentucky. buys it
- P1 new state, 1000$ 1 property

### Feedback loops
When result of a system interaction feeds back into system to generate a new interaction
- Positive (accentuates action)
- Negative (diminishes action)

**Positive feedback**
A change in the system that augments likelihood that the change will happen again
-> amplification

Main pro and con:
- Useful to get things over quickly once a side has taken an advantage
- Runaway winner or slippery slope

Ex: 
RPG fight
- Character gets hit, is stunned for a few seconds
- Because he is stunned, he is easier to hit
- Gets hit again, stunned again
- Etc.


**Negative feedback**
A change in the system triggers a counter-balancing change in the system
-> Stabilisation

Main pro & con:
Useful to allow reversals in a game
Can prolong games indefinitely

EX: UNO
- you have almost no cards left, close to winning
- You have less opportunities to play your caards, end up picking up new cards
- Opponents with many cards can control the game and make you pick up cards
EX: Thermostat
- Temperature drops, thermostat turns heater on
- Temperature rises, thermostat turns heater off

One can track feedback loops in system and fine-tune the interaction between the types to make play as enjoyable as possible

### Emergence

**INSERT WIKIPEDIA DEF HERE**

Ex: Conway, Life (1970)
Only 4 rules:
- Each living cell with one or no neighbours dies, as if by solityde
- Each living cell with four or more neighbours dies as if by ovepopulaiton
- Each living cell with two or three neighbours survives
- 

Ex: Chroniqueur
- Reluctant serial killers: drunk people at feasts can accidnetally kill someone, gets a little better at killing, vendettas are generated from family members and try to kill killer, but killer is better at killing and kills them, generating more vendettas
- Thieving hermits
- Eternal chiefs
- Micro-weddings: Small communities, so one needs to get married, for drama, one has certain preferences, 
- Hereditary casanovas: Quests can get passed on to descendants, people can have crushes on someone and want to seduce them, these are quests, sometimes someone ends up with multiple seduction quests passed on from various descendants

## Game balance
Games are alive, have behaviours, need to be balanced
"balance" is a general lotion, can mean many different things
generally, dynamics bseem to behave according to certain expectations
What are these expectations?
- Fairness?
- Equal chances?
- Flow?

**Fairness**
Ethos: May the best one win
Problems:
- One side has an advantage (starting first, better units, etc.)
- Victory is dependant on external factors (chance)
Solutions:
- Counterbalancing advantages
- Removing or attenuating chance

**Equal chances**
Ethos: Everyone has a chance to win
Problems:
- Experienced players always win
- Adults always win
Solutions:
- More chance or chaotic factors
- More accessible mechanics
Ex: Drawful
Drawing games v skill-based, but drawful gives you points for lots of other things

**Flow**
Ethos: Difficulty is always just right
Problems:
- Difficulty is super subjective
Solutions:
- Design for a specific kind of player
- Offer difficulty levels
- Dynamic difficulty adjustments
Ex: Matchmaking, could also work for equal chances

**Variety**
Ethos: One can play in many different ways
Problems:
- One way is just better
Solutions:
- Buff and nerf components until strategies are just right

**Investment**
Ethos: The more you play, the more you get
Problems:
- Reaching skill plateaus
- Getting stuck
Solutions:
- Reward participation, not achievement
## Recap
Mechanics allow stuff to happen,
Dynamics are the stuff that happens
The loops are what
Systems are a top-down overview, allow you to track things as they go
