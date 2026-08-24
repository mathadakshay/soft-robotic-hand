# Soft Robotic Hand

A 3D-printed tendon-driven robotic hand developed as a 3-member team project for demonstrating Edge, Top, and Wall grasping strategies.

## Project Overview

The objective of this project was to design, manufacture, assemble, and control a soft robotic hand capable of grasping lightweight objects and placing them into a designated box.

The demonstrated grasping tasks were:

- Edge grasp: flat objects with a maximum height of 10 mm
- Top grasp: objects within approximately 100 × 80 × 200 mm
- Wall grasp: cylindrical objects of approximately Ø40 × 200 mm
- Object pickup and placement with repeated successful trials
- Object mass below 200 g

## Mechanical Design

The hand was designed and iterated in SolidWorks

The mechanical system combines:

- TPU 3D-printed finger joints for compliant movement
- PLA components for structural parts
- PTFE/Teflon tubes for tendon guidance
- Tendon-driven finger actuation
- Dynamixel XL330 motors

A major design consideration was ensuring that the components could be assembled after 3D printing, particularly around motor mounting, underarm structure, tendon routing, and access to small assembly features.

## Actuation System

The final prototype uses four Dynamixel XL330 motors.

| Actuator | Function |
|---|---|
| Motor 0 | Thumb right/left movement |
| Motor 1 | Index finger actuation |
| Motor 2 | Middle finger actuation |
| Motor 3 | Ring finger actuation |

The exact motor mapping and motion parameters are documented in the `hardware/` directory.

## Grasping Strategies

### Edge Grasp

The thumb and index finger are used to grasp thin, flat objects from the edge.


### Top Grasp

The fingers wrap around the object from above.


### Wall Grasp

The hand uses the surrounding wall/contact surface while grasping a cylindrical object.



## Control

The hand is controlled using Python and the Dynamixel interface.

The control system was based on a professor-provided framework and adapted for the final hardware configuration, motor mapping, position limits, and grasping sequences.

The repository contains the experimental control code and motor-testing notebooks.

## Design Iteration

One of the main engineering challenges was translating the CAD design into a physically assemblable mechanism.

Several iterations were required to improve:

- Motor mounting
- Underarm geometry
- Finger-joint design
- Tendon routing
- Assembly accessibility
- Component clearances

## My Contribution

This was a collaborative 3-member project.

My main responsibilities included:

- Developing and iterating finger and hand concepts in SolidWorks
- Refining the mechanical design based on assembly requirements
- Supporting the development of the underarm and motor-mounting design
- Assembling the 3D-printed hardware
- Routing and integrating the tendon system
- Adjusting the design based on physical testing


## Key Engineering Lessons

The project reinforced the importance of designing not only for functionality, but also for manufacturing and assembly.

A major takeaway was the iterative relationship between:

**CAD → 3D Printing → Assembly → Testing → Design Modification**

## Technologies

- SolidWorks
- Python
- Dynamixel XL330
- 3D Printing
- TPU
- PLA
- PTFE/Teflon tubing
- Tendon-driven actuation

## Project Status

Completed as a team-based robotics development project.
