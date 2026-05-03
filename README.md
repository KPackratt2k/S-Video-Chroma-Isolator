# S-Video-Chroma-Isolator
An optocoupler circuit for adding an S-Video input on hot chassis CRT TVs.

Primarily designed for 80s era Sony CRT TVs utilizing the P3 family of chassis, this mod can be adapted for use with any hot chassis CRT TV that has AV inputs and a jungle chip with a separate Chroma input. The Chroma coupling circuit is based on the Composite video isolation circuitry of a Daewoo CRT TV of an unknown model, utilizing off-the-shelf components for simplicity.

> [!CAUTION]
> CRT displays can carry very high voltages, even when powered off. Make sure you are familiar with safely working inside a CRT TV before proceeding. Proceed at your own risk!

----------

## Boards
There are three boards in this repository. In most cases, you'll only need to use the main optocoupler board (Sony P3 Chroma Isolator) for these mods. The other two (Sony P3 S-Video Switch and Sony TS20 S-Video Shield Coupler) are intended for use with Sony P3-A chassis TVs (KV-20/27TS20-26) to replicate the S-Video switching circuit from the KV-27TS30 for a factory-like functionality on these TVs.

OSH Park links:
- [S-Video Chroma Isolator](https://oshpark.com/shared_projects/XefR2KEe)
- [S-Video Switch for Sony P-3A Chassis](https://oshpark.com/shared_projects/bug9zkJt)
- [S-Video Shield Coupler for Sony P-3A Chassis](https://oshpark.com/shared_projects/kqW87HR9)

----------

## Installation
Installation instructions will vary based on the TV you are working on. Instructions for models that have been tested to work with this modification will be posted in this repository soon. Here's a short description of each connection label on the optocoupler board for assisting with installation:

- GND (Hot Side): Ground on the hot side of the AV isolation circuit on the TV chassis.
- VCC (Hot Side): Power rail (usually 8-12V) for the hot side of the AV isolation circuit on the TV chassis.
- GND (Cold Side): Ground on the cold side of the AV isolation circuit on the TV chassis (closest to AV inputs).
- VCC (Cold Side): Power rail (usually 8-12V) for the cold side of the AV isolation circuit on the TV chassis.
- C_IN: Input for S-Video Chroma pin on the Mini-DIN jack.
- C_OUT: Isolated S-Video output for running to a switch.
- YCJ_IN: For connecting the Chroma input of the TV jungle chip to a switch.
- TV_C: For connecting the original RF and Composite Chroma circuitry of the TV to a switch.

You'll have to cut the connection between the factory Chroma processing circuit for the stock AV inputs and the Chroma input pin of the Jungle chip and use a switch to toggle the inputs. There are two sets of JST connectors connected together on the bottom-right corner of the board to simplify the connection between the TV circuitry and the switch.

It is strongly recommended to use shielded wire for the Chroma I/O connections of the TV, as using regular unshielded wire can cause interference which can prevent the mod from working properly.

The Luninance (Luma) component of the S-Video Mini-Din connector goes directly to the Composite video input of the TV.

----------

## Todo
This repository is a work in progress. The following tasks will be done soon:
- Write installation instructions for the tested models.
- Mirror the Bill-of-Materials from the OSH Park links as text documents inside the repository.
- Design 3D printed mounting brackets for the PCBs to simplify installation.
- Redesign the TS20 mod to consolidate the three PCBs into one for cost optimization.

----------

## Credits:

- The Shmups Forum
- Andy King
- Matt Ross (6tanks)
