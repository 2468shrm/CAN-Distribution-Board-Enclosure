# CAN-Distribution-Board-Enclosure

This repo inclues the design for a 3D-printable enclosure for the
CAN-Distribution-With-Debug and CAN-Distribution-Board-With-Power-v2 PCBs
to make mounting easier on FRC robots.

The enclosure for a board is assembled from 2 or 3 3D printed parts:
- Bottom - Always needed, it goes below the PCB
- Top - Always needed (or Top for Debug), it goes above the PCB.  There are a couple of
options for tops available, one should be selected and used.
  - (Normal) Top - includes openings for termination headers.
This is used when enclosing the CAN-Distribution-Board-With-Power-v2 PCB.
  - Low profile Top - does not include an opening for termination headers and is a lower
profile (less height) enclosure. This is used when enclosing the
CAN-Distribution-Board-With-Power-v2 PCB.
  - Top for debug - includes openings for debug elements and termination headers.
This is used when enclosing the CAN-Distribution-With-Debug PCB.
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

# Identification and Association of the Connectors and Signals

To avoid mistakes in robot wiring, it is recommended that the connectors be identified
similarly to the REV, NI and CTRE hardware.  NI and CTRE uses Weidmuller connectors
and they typically identify CAN connections on the enclosure of the product.  REV gets
WAGO connectors pre-colored by the factory.

## Identification Conventions

The standard used by the existing CAN-device vendors use one of two methods.  CAN wire is
universally a twisted pair of yellow/green wire ().  The yellow is CAN_H and the green
is CAN_L.  If color is not used connectors are labeled H and L (in some cases both color 
and letter are both used).

At 2468, to remember which is which, we say "the yellow sun is High in the sky, but the
green grass is Low in the ground."

## Identifying Connections on the CAN Distribution Board

We have found that medium tipped Sharpie pens are useful for coloring the WAGO 250-series
connectors.  We normally color the plastic below the opening for the wire down to the PCB.
Coloring is straight forward because the connector is stacked up and seams exist between
inputs, providing "lines" to color within.

This image shows two enclosures, one with attached low-profile top and one without top. Both
include connectors colored with sharpies to indicate the purpose of each connection.
![alt text](https://github.com/2468shrm/CAN-Distribution-Board-Enclosure/blob/main/IMAGES/SharpieColoredConnectors.jpeg?raw=true)

We are also experimenting with the use of laser-printed decals. The decal paper is
purchased from Amazon and craft stores. Each CAN Distribution Board requires a set of
four decals, one per WAGO 250-204 connector. We believe the decal can be applied to
the connector in the same region as the sharpie color in, however we will also experiment
with adding a decal on the enclosure plastic (top) in front of the WAGO connector.

The set is shown below, but
[PDF](https://github.com/2468shrm/CAN-Distribution-Board-Enclosure/blob/main/Decals/CAN%20Distribution%20Board%20Decals.pdf)
and [SVF](https://github.com/2468shrm/CAN-Distribution-Board-Enclosure/blob/main/Decals/CAN%20Distribution%20Board%20Decals.svg)
files containing a large number of sets is available in the repository.

![alt text](https://github.com/2468shrm/CAN-Distribution-Board-Enclosure/blob/main/IMAGES/Decal%20Pattern.png?raw=true)
