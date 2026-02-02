# Mechanical design

## Design progress
- [ ] base
- [ ] turntable
  - [ ] plate
  - [x] gear
- [ ] shoulder joint
- [ ] major arm segment
- [ ] elbow joint
- [ ] minor arm segment
- [ ] arm termination


## Overview

- 3 axes of rotation
  - turntable with 1:9 ratio
  - two arm joints with 1:5 ratio
  - $\therefore$ two arm segments (major and minor)
- rotational joints are belt driven from NEMA17 stepper motors
  - steppers fitted with metal gears of ~12.8 mm pitch diameter and 20 teeth
- mounting plates for hand and camera attachments


## Main mechanical components

### Base
- TODO

### Turntable
- plate ~ 150 mm diameter
  - laser ply
  - stepped turntable radius
    - limits range of rotation with physical endstop
    - provides homing to centre of rotation with optical switch
  - through hole at centre for wiring
  - mounting holes for
    - turntable gear
    - shoulder joint bracket and shoulder stepper bracket
    - lazy-susan bearing
- gear
  - 3D print
  - 1:9 ratio $\to$ 115.2 mm pitch diameter and 180 teeth
  - bolted to underside of turntable plate
  - lip to keep belt aligned
 
### Shoulder joint
- bracket
  - 3D print
  - single piece? that sits around the wiring through hole in the turntable
  - bolted pillow blocks for bearings(8mm inner, 19mm outer, 6mm depth)
- gear
  - 3D print
  - mounts to major arm segment side panel
  - 1:5 ratio $\to$ 64 mm diameter and 100 teeth

### Major arm segment
- side panels
  - 50 mm square cross-section
  - approx 243 mm length ?
  - compressed into diagonal spacers (see below) using nuts on threaded bolts
  - one side with homing slot for shoulder joint optical switch
  - other side with mount point for shoulder joint gear
  - axel is smooth rod (d=8mm) that is fitted into both bearings (potentially with tolerance rings)
    - clamped by gear on one side and ply cap on other, through holes in the side panels of the arm segment
- diagonal spacers
  - slanted at 45deg - square projection in cross-section direction

### Elbow joint
- TODO

### Minor arm segment
- side panels
  - largely similar design to the major arm segment
- TODO mount point for arm termination plate
- TODO mount point for camera module?

### Arm termination
- square plate
  - laser ply - 3 mm
  - four M3 mounting holes for e.g. hand attachment

## Links and other notes

- [belt length solver](https://www.desmos.com/calculator/8e1lo7mxcq) - we bought fixed length belts so need to find the gear separation distance for given gear radii
