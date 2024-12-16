# IRIS-2 Hardware
IRIS-2 is a 5 kg video and imaging instrument built by a group of friends (formed by enthusiastic amateur astronomers, engineers, and technicians). It follows the legacy of IRIS-1, which flew on Sunrise II in 2013. Its main goal is to provide imagery for communication and outreach, while also assisting in monitoring and improving the mechanical interfaces and PCS of the [Sunrise III observatory](https://www.mps.mpg.de/solar-physics/sunrise) from launch through landing and recovery. The cameras record 4K, 30 fps video for 2 hours during launch, 1 hour during landing, and 15 minutes at 120 fps during balloon release. At other times, they capture stills at 120-second intervals for time-lapse creation.

IRIS-2 was designed and assembled by:
* [Ramón García](https://github.com/rgalarcia/)
* [Miguel Angel Gomez](https://x.com/haploretro)
* [David Mayo](https://github.com/dmay0/)
* [Aitor Conde](https://github.com/bultza/)

To know more about the [Sunrise solar observatory](https://www.mps.mpg.de/solar-physics/sunrise)

## Design
IRIS-2 is build around 4 battery-less GOPRO Hero 4 cameras, with a central computer build with a MSP430 FRAM based microcontroller. The Instrument should be:
* Power independant
* Fully autonomous to detect launch and landing
* Able to make 4K videos
* Able to make a full timelapse of the flight of Sunrise over 7 day
* Able to stay in standby for days while drawing as less energy as possible.

## The hardware
The hardware has been designed using Altium Designer 21. The instrument has 2 boards (CPU and interface board), 4 cameras and a battery pack:
* The [IRIS2_PCB_CPU](https://github.com/bultza/IRIS2-hardware/tree/main/IRIS2_PCB_CPU): Where all the magic happens.
* The [IRIS2_PCB_Frontplate](https://github.com/bultza/IRIS2-hardware/tree/main/IRIS2_PCB_FrontPlate): a PCB to interface the instrument with the exterior world.
* 4 "GoPro HERO 4" cameras
* 4 [MewPro 2](https://mewpro.cc/en/product/mewpro-2/) interface boards to control the cameras
* 56 NiMH Eneloop AA cells, (8 in parallel, 7 in series)

![IRIS-2 Block Diagram](https://github.com/bultza/IRIS2-hardware/blob/main/IRIS2_PCB_FrontPlate/docs/IRIS2.png)

## Pictures
IRIS-2 in action:
![Sunrise III image taken by IRIS2](https://github.com/bultza/IRIS2-hardware/blob/main/doc/2024_sunrise_3_composition.jpg?raw=true)

IRIS-2 Mounted on Sunrise III
![IRIS-2 Mounted on Sunrise III](https://github.com/bultza/IRIS2-hardware/blob/main/doc/IRIS_mounted.jpg?raw=true)

## Flight Software
The software for this mission is at a different repository that can be found here: https://github.com/bultza/IRIS2-firmware-flight. It contains:
* The flight software
* The scripts to read and translate the Events to Human readable text
* The scripts to load the telemetry into a influx database for later usage on a Grafana dashboard 

## Authors
This was done using invaluable time from my friends. We all contributed to the success of this mission:
* [Ramón García](https://github.com/rgalarcia/)
* [Miguel Angel Gomez](https://x.com/haploretro)
* [David Mayo](https://github.com/dmay0/)
* [Aitor Conde](https://github.com/bultza/)

## License
This project is licensed under the CERN Open Hardware Licence Version 2 - Weakly Reciprocal (CERN-OHL-W). You can find the full text of the license in the [LICENSE](LICENSE.md) file in this repository or at the [CERN OHL website](https://ohwr.org/project/cernohl/wikis/home).

Please ensure that any use or modification of this project includes the following notice:
"Original design by [Daedalus Team/IRIS-2 Instrument]. Modifications must be shared under the same CERN-OHL-W license."

Under this license, you are free to use, modify, and distribute this hardware design. If you modify the design and distribute your changes, you must make those changes available under this same license.
