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
* Able to make a full timelapse of the flight of Sunrise over 7 days

## The hardware
The hardware has been designed using Altium Designer 21. There are two boards, each on a sub-folder in this repository:
* The IRIS2_PCB_CPU: Where all the magic happens.
* The IRIS2_PCB_Frontplate: a PCB to interface the instrument with the exterior world.
Each folder has a "docs" folder with all the datasheets, pdf and gerber files to build it yourself

## Pictures
A composed picture made by the 4 cameras during the flight
TBC

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
  
