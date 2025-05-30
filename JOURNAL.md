---

title: "Modular RC Car Platform"
author: "Knivier"
description: "A modular, Raspberry Pi-based RC car with long-range control, vision, LiDAR, and future wireless charging."
created\_at: "2024-03-20"
-------------------------

## 2024-05-20

**Entry:** Initial brainstorming session.
I started defining the scope of my modular RC car project today. The goal is to create a two-phase RC car build: Phase 1 will involve basic chassis, drivetrain, and remote control; Phase 2 will integrate autonomy features like a camera, LiDAR, and wireless charging prep. I'm targeting under \$150 for Phase 1, and under \$350 total. The car will be about the size of a Traxxas RC truck, capable of some off-road use, and built around either a Raspberry Pi or Arduino.

## 2024-05-21

**Entry:** Component and architecture planning.
I sketched out the hardware architecture today. I decided on using a 4WD skid-steer chassis for simplicity, driven by 4 TT motors via dual H-bridge drivers. I'll use a Raspberry Pi for Phase 2 processing, but Phase 1 will probably use an Arduino for basic PWM motor control. A FlySky FS-i6 radio system will handle remote input. For power, I’ll use a 3S LiPo battery (\~2200mAh) for a balance between runtime and weight.

## 2024-05-22

**Entry:** Researching modular chassis options.
After digging through forums and sites, I found some robust yet budget-friendly options like the HiWonder aluminum 4WD kit. It comes with durable brackets and pillars for layering electronics. I also confirmed that the kit can support small off-road use with proper tires and motor gearing. Planning to mount components in stacked plates to keep everything modular and easy to upgrade.

Some auton notes include it now will likely need to be run on a raspi and not an arduino; LiDAR and vision systems will take lots of processing power.

## 2024-05-23

**Entry:** Planning for power system integration.
Looked into LiPo and NiMH packs for power. Leaning towards a 3S LiPo for compact size and good output, paired with a buck converter to give me stable 5V for logic systems. I diagrammed a basic power flow: battery → switch → voltage regulators → Pi/Arduino + Motor Drivers. Planning ahead, I’ll keep enough spacing under the chassis for future wireless charging coil installation.

## 2024-05-24

**Entry:** Control system planning.
Confirmed that the FlySky FS-i6 radio system can directly interface with the Arduino for Phase 1. I’ll wire the receiver outputs into digital pins and decode PWM to control the motors. Planning to use the TB6612FNG dual H-bridge modules – they’re compact and efficient. In Phase 2, I’ll switch the Pi in as the main controller and reroute signal interpretation through a Python interface.

I'm also looking into AA batteries that are rechargable, with a buck converter for power. Alternatively I can make my own small battery pack.
## 2024-05-25

**Entry:** Phase 2 tech roadmap.
Planned the Phase 2 upgrades. I’ll add the Raspberry Pi Camera Module v2 and an RPLIDAR A1 for autonomous nav experiments. For wireless charging, I’m investigating a Qi receiver module and custom positioning pad. The top plate will have mounting holes ready for the LiDAR bracket, and a servo mount for a camera pan/tilt setup.

## 2024-05-26

**Entry:** Assembly planning and modular design philosophy.
Outlined modular design requirements. Each subsystem (drive, logic, power, sensors) will be isolated with quick-disconnects: JST or servo connectors for motors, USB or ribbon cables for peripherals. I’ll 3D-print or cut modular boards that mount atop the chassis using standoffs. This way, I can upgrade components like the Pi or LiDAR without rewiring the whole vehicle.

## 2024-05-27

**Entry:** Outdoor usage considerations.
Planned for outdoor performance – added waterproofing as a future upgrade (e.g., waterproof ESC, sealant for electronics). Selected a tire style suitable for light gravel, grass, and asphalt. Will raise the electronics deck slightly above the motors and cover it with a splash shield. Left space for heatsinks or small fans in case components run hot under the sun.

## 2024-05-28

**Entry:** System integration mapping.
Sketched a system block diagram showing all components: battery, power rail, motor drivers, controller, sensors, and remote receiver. Will build Phase 1 with headers and labels for all GPIO lines so Phase 2 sensors can just plug in. Planning to use ROS 2 in Phase 2, so Phase 1 code will follow best practices to ease that migration later.

## 2024-05-29

**Entry:** Materials list and sourcing.
Compiled a rough BOM for both phases. The first phase comes in under \$150 with room for better tires or a better frame. Found affordable options for everything on Amazon, Adafruit, and AliExpress. Phase 2 BOM caps at \~\$350 with the RPLIDAR A1, camera, Qi pad, and upgrades. Documented the vendors and shipping times to start ordering this weekend.

Engineering teacher one on one soldering started today, building a random number generator.
## 2024-05-30

**Entry:** Finalized Phase 1 layout.
Finalized the layout for Phase 1. Electronics will be arranged in a stacked configuration: motors and driver on the baseplate, power and Arduino on mid-layer, and receiver on top. Made a wiring plan with color coding and quick connectors for easy debugging. Next week, I’ll begin building and soldering Phase 1. Forgot to push all my journal entries so I did that. 

Random generator capacitors resistors and light bulbs complete, headers yet to be soldered, I think I might be ready to solder personally. Will require prior setup in terms of solder tools, I am willing to spend money for that though.
