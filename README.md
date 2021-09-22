
# Starbase Ship Designs

Decker's Ships; Donations are appreciated :).

## Vigil-EmptyFrame.fbe - testing engine module structure; modifications in progress, required radiators, and the 

actual built version had to be manually modified; need to remove some thrusters(?).

- Thrusters, generator, cockpit; how fast is the fastest thing?  *spoiler - depressingly slow compared to everything else*
- 526,513kg, 15TMR

## Vigil-ResearchVessel.fbe (Vigil RV)

Initial upgrade of vigil frame to support some utility, and beams to support rigid bolting of ore onto the sides (ore is 5:4 ratio of size, sortof).

- 40 working crates
- beam structure for bolting extra ore - 120 extra slots (4*20+4*10).
- 2 mining lasers 1 ore collectr
- 2 tractor beams
- 3 spots to mount cargo locks (empty frames, never completed the mods on the BP)
- warp core
- requires a crafting bench or 2 mounted for balance.
- long distance
- 3,583,140kg, 7.9TMR empty, 5.4TMR cargo full, less with ore bolted to frame.


## Vigil-BoxFrame (Vigil BF)

Replaces beams with cargo lock frames that can hold ore instead - single button locks and unlocks; 

- 40 working crates
- 256(54*4+4*9) ore in cargo frames; frames are slighly larger than ore blocks and other things like warp cores or thrusters
could be carried.
- quad ISAN2
- 2 mining lasers 1 ore collector on syncrhonized turrets
- warp core
- requires a crafting bench or 2 mounted for balance.
- long distance
- 4,891,903kg, 6.6 TMR empty, full is hard to measure

## RingOfFire-base

Ring Of Fire - 1 ring of thrusters, and maneuvering thrusters, rough dual mode cockpit with beams to sense
pilot in seat... (fails under high rotation rates in certain directions).  

- 576 cargo crates
- 24 mining lasers (100 weapon points)
- 6 ore collectors,
- 4*24 (96) t2 box thrusters for main engines, 8 downup/down 8 left/right (16 roll).
- 600km distance or so
- 13M kg, 2.4TMR empty, 1.3 40k crate load.


## RingOfFire-RC1 

Ring Of Fire - dual ring of thusters (192)

- 600 cargo crates
- warp core
- 24 mining lasers (100 weapon points)
- 6 ore collectors,
- 4*24 (96) t2 box thrusters for main engines, 8 downup/down 8 left/right (16 roll).
- 1500km distance empty
- 16.5M kg; 6.2 TMR empty, 2.6 max load (no ore is max load in 1728v).
- 60 min before replacing fuel rods (about 600k km at top speed)

## Ring of Fire - First Build

Actual build of fast, max part ring of fire ship; some of the thrusters are misnamed, multiple FCU's cause drastic issues in Real server...
extra lag for controlling ship encountered... sort of figured things would stabilize; rapid acceleration causes radical jerks for no good reason (leverage of thrusters?)

- Same as specs of RC1; added resource bridges, tried to separate engine rings to have separate scalars - even disable a ring entirely to save on fuel while mining.


## Ring of Fire - Fixed Engines

The clone/rotate function of SSC ate one of the pipe segments on 2 engine blocks; this has that fixed - needs MFC fixed... I have a module for it- (version built for ticket)

## Ring of Fire - V2 

Alternate Balance - moves the CoM nearly 4m behind CoT; improved power system, manual/auto sweep mining, a couple different patterns for mining lasers firing order.

Improved fuel capacity and 2x refuel available; prioritized battery management.

- [Owners Manual](Rof-OwnersManual/RingOfFire.md)

![Example Image](RingOfFire.jpg)
![Example Image](RingOfFire-InFlight.jpg)




## Dart - V1

- 128M propellant (31 hours) (114M Excess propellant for 3 hour trip)
- 27 thrusters 
- 6.21TMR
- 8 Fuel Chambers, 8 Generators, 8 spare fuel rods (3 hours)
- Avoidance Script
- Origin Compass Script
- Single Receiver ISAN
- Smarter Battery Charge Script

![Dart](DartV1Cost.jpg)
![Dart](DartV1-Internals.jpg)

### Initial version

![Dart](DartV1Side.jpg)
![Dart](DartV1Top.jpg)

## Dart W - V1

- Adds warp core, removes 32M propellant (96M) to keep TMR>6.

![DartW](DartW-V1.jpg)

## Dart 192

Increases propellant slightly - realized I already had twice what I meant to have... 
adding double again dropped the TMR to 5.35.

192M propellant, 8 fuel chamber 8 generator, 21 thrusters, 6.1TMR




# Changelog

- Ring of Fire(V2) Updated, strength factor 32; fixed missing pipe on thruster(R3), fixed flight status lockout, fixed fuel scripts, export x, y, z, speed variables from ISAN, shows estimated time to empty better.
- Dart-V1 removed enhancers since speed is the only purpose of the thing; developed improved battery managment script.