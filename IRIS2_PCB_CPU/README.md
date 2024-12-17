# IRIS2 CPU PCB
This is the IRIS2 CPU PCB design for the IRIS2 instrument that has flown twice, during the Summer 2022 and the Summer of 2024. The PCB Contains:
* A Central low power with flight heritage MCU: MSP430FR5994
* A pressure Sensors to measure the altitude of the instrument above the surface
* Four independent DC-DCs to power the GoPro Cameras
* A Current and voltage monitor
* A 3 axis accelerometer to detect Free-fall
* A NOR flash memory to save all the telemetry and event logs
* A RTC clock in order to be able to track down the telemetry

The project was built using Altium Designer 2021 version.

![IRIS-2 CPU from the top](https://github.com/bultza/IRIS2-hardware/blob/main/IRIS2_PCB_CPU/docs/IRIS2_CPU_PCB.jpg?raw=true)

## Documentation
Relevant documentation can be found on the docs folder including the datasheets of all the components:
* [Block Diagram](https://github.com/bultza/IRIS2-hardware/blob/main/IRIS2_PCB_CPU/docs/IRIS2_CPU.png)
* [Schematics PDF](https://github.com/bultza/IRIS2-hardware/blob/main/IRIS2_PCB_CPU/docs/IRIS2_PCB_CPU_v1.3.pdf)
* [Pinouts](https://github.com/bultza/IRIS2-hardware/blob/main/IRIS2_PCB_CPU/docs/IRIS2_pinouts.xlsx)
* [3D Step File](https://github.com/bultza/IRIS2-hardware/blob/main/IRIS2_PCB_CPU/docs/20210401_IRIS2_PCB_CPU.step)
* [The User manual & Software](https://github.com/bultza/IRIS2-firmware-flight)

![IRIS-2 CPU Block Diagram](https://github.com/bultza/IRIS2-hardware/blob/main/IRIS2_PCB_CPU/docs/IRIS2_CPU.png?raw=true)

## Authors
https://github.com/bultza/IRIS2-hardware/tree/main

