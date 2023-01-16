# CAN-Distribution-Board-Enclosure

This repo inclues the design for an enclosure for the CAN-Distribution-With-Debug
and CAN-Distribution-Board-With-Power-v2 PCBs to make mounting easier on FRC robots.

The enclosure for a board is 2 or 3 parts:
- Bottom - Always needed, it goes below the PCB
- Top - Always needed (or Top for Debug), it goes above the PCB.  There are a set of
tops available, one should be selected and used.
  - Top for debug - includes openings for debug elements and termination headers.
This is used when enclosing the CAN-Distribution-With-Debug PCB.
  - (Normal) Top - includes openings for termination headers.
This is used when enclosing the CAN-Distribution-Board-With-Power-v2 PCB.
  - Low profile Top - does not include an opening for termination headers and is a lower
profile (less height) enclosure. This is used when enclosing the
CAN-Distribution-Board-With-Power-v2 PCB.
- Termination Top - An optional item for Tops that expose a pair of headers for CAN
termination.  The Termination Top is used to cover/block the termination header opening
in the Top. Needed only if the termination headers are installed but not used
and the opening is to be blocked.

The Bottom and Top are screwed together using M2 hardware.  The enclosure is connected
to the robot using 8-32 screws.

As assembled, the enclosure is as follows:

![alt text](https://github.com/2468shrm/CAN-Distribution-Board-Enclosure/blob/main/IMAGES/Assembly.png?raw=true)

Note: This is with Top (no debug features populated on the board) and the Termination Top
is installed.

## Bottom

A very simple base/bottom of the enclosure.  The bottom requires you to press in 3
heat set inserts.

The bottom uses 3 M2 heat set inserts to connect with screws from the top to hold the
two halfs together.
- McMaster [94180A307](https://www.mcmaster.com/catalog/94180A307)


![alt text](https://github.com/2468shrm/CAN-Distribution-Board-Enclosure/blob/main/IMAGES/Bottom.png?raw=true)

## (Normal) Top

A very simple top of the enclosure. The termination header window is included. To block it,
use the Termination Top.

![alt text](https://github.com/2468shrm/CAN-Distribution-Board-Enclosure/blob/main/IMAGES/Top.png?raw=true)


## Low Profile Top (No Termination or Debug windows)

A low-profile (low height) top for the enclosure. It is the preferred version for 2468 in
FRC applications as it should minimize debris/swarf from entering the enclosure.

This top allows the enclosure to be assembled with a 10 mm M2 screw.
- McMaster [92095A104](https://www.mcmaster.com/catalog/92095A104)

![alt text](https://github.com/2468shrm/CAN-Distribution-Board-Enclosure/blob/main/IMAGES/WithLowProfileTop.png?raw=true)

## Top for Debug

The same as Top, but with windows for debug hardware (power block and a light pipe to
transmit the LED to the top.

![alt text](https://github.com/2468shrm/CAN-Distribution-Board-Enclosure/blob/main/IMAGES/Top%20for%20Debug.png?raw=true)

## Termination Top

The termination top is used for Tops (normal and debug) when the termination headers should
be covered to avoid debrus/swarf from entering the enclosure.  The Termination Top is
expected to be glued to the top (e.g. super glue).

![alt text](https://github.com/2468shrm/CAN-Distribution-Board-Enclosure/blob/main/IMAGES/Termination%20Top.png?raw=true)

