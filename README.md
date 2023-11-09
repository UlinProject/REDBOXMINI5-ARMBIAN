# REDBOXMINI5-ARMBIAN
All technical information about the REDBOX MINI 5 device, including the ability to build the Linux ARMBIAN distribution.

<b><i>!!ATTENTION!!</i></b>

<b><i>// The data in this repository is experimental and may contain errors. I do not provide ready-made assemblies; it is up to the user to decide whether to use this data or not, to collect an image to run third-party software or not.</i></b>

<b><i>// This repository was originally developed only for V1, later only the V2 version was added. Versions with less RAM and permanent memory and a different processor were not considered.</i></b>

### Board versions:
## V1:
<b>CPU:</b> Allwinner H5 (AArch64, x4, 0.2Ghz-0.912Ghz <b>(1.01 GHz works too)</b>)

<b>MEM:</b> 1GB (DDR3, 336.00 GHz - 672.00 GHz <b>(1344.01 GHz works too)</b>)

<b>Eth:</b> Internal (100mbit)

<b>WI-FI:</b> XR819 (was not considered)

<b>EMMC:</b> Q2J55L (7.09 GiB) (works, installation is not guaranteed)

<b>GPIO:</b> LED_PWR (1c20800, 15-PA15), LED_STATUS (1f02c00, 362-PL10), IR (1f02c00, 363-PL11), KEY_RESET (1f02c00, 355-PL3) (On this board you can get absolutely any gpio that is available on allwinner h5 (I’m just giving a list of those pins that you can get without much effort).)

## V2:
<b>CPU:</b> Allwinner H5 (AArch64, x4, 0.2Ghz-0.912Ghz <b>(1.01 GHz works too)</b>)

<b>MEM:</b> 1GB (DDR3, 336.00 GHz - 672.00 GHz <b>(1344.01 GHz works too)</b>)

<b>Eth:</b> Internal (100mbit)

<b>WI-FI:</b> XR819 (was not considered)


### Quick answers to questions:

#### Will there be support for 1.2/1.5 GHz processor frequencies?

These set-top boxes do not have an adjustable VDD-CPUX regulator (either using a GPIO transistor or an i2c regulator) and use a constant voltage of 1.1V to operate. This does not improve power savings or increase the supply voltage to 1.3V in situations where it is needed.

#### Will there be WI-FI support?

Not at the moment due to the difficulty of obtaining working and up-to-date driver source code. Also, this chip is not very productive and preference remains for wired eth or usb wifi.
