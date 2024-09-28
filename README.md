# Torex XC9148 Breakout Board

> [!WARNING]
> The information and material (code, designs, files, ...) are provided "AS IS". We make no representation or warranty of any kind, express or implied, regarding the accuracy, adequacy, validity, reliability, availability, or completeness of any information or material. Use this at your own risk.

> [!WARNING]
> At the time of writing this PCB has not even been produced yet, and as such, it has not even been tested yet! Once it has been properly tested, I will confirm that everything works as expected.

> [!WARNING]
> This board was designed for the XC9148G50CER variant of the XC9148. This has some characteristics that are important for the design of this breakout board (e.g. its output voltage, oscillation frequency and lack of bypass mode). 


## Introduction

This is a breakout board for the Torex XC9148 voltage convertor.

[https://product.torexsemi.com/en/series/xc9148](https://product.torexsemi.com/en/series/xc9148)

<img src="images/pcb.png" width="600">

## Change Log

* v1.0
  * Initial design 

## Design Considerations

* Designed specifically for the XC9148G50CER variant of the XC9148
  * 0.9 - 6V input  
  * fixed 5V output
  * 1.2MHz oscillation frequency
  * no bypass mode

## Schematics 

<img src="images/schematics.png" width="600">

## How to Obtain the Physical PCB

<img src="images/pcb.png" width="600">

The Gerber file is in this repository (`kicad/gerbers/XC9148-breakout.zip`). Simply upload this file a PCB manufacturer of your choice (JLPCB, PCBWay, ...), and you they will make it for you for as low as \$5 for 5 pieces (with the cheapest shipping option, which can take a few weeks).

For JLCPCB, select the order number option where they will replace "JLCJLCJLCJLC" on the board with the actual order number.

> [!WARNING]
> Note that will still have to solder the components onto the PCB yourself!


## How to Edit Design

Everything you need to edit this design in KiCad 8 is included in the repository.

However, this project uses symbols, footprints and 3D models from [Component Search Engine](https://componentsearchengine.com/). Their license allows us to do pretty much whatever we want with them, except redistributing them. For this reason I can't include them in this repository.

If you would like to edit the design yourself, you will need to download the following component libraries from [https://componentsearchengine.com/](https://componentsearchengine.com/) (it's free!):

* [https://componentsearchengine.com/part-view/XC9148G50CER-G/Torex](https://componentsearchengine.com/part-view/XC9148G50CER-G/Torex)


From the downloaded zip files, move the content of the `KiCad` and `3D` subfolders into the project structure, so that the end-result looks like this:

<img src="images/project_structure.png" width="300">

The KiCad project is configured to look for these files in these locations, using relative paths, so no changes to the project itself are required.	

## Sources

* [https://product.torexsemi.com/en/series/xc9148](https://product.torexsemi.com/en/series/xc9148)
