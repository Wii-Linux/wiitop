# WiiTop Specification (prototype - Rev E)

The WiiTop will be a Wii in the form factor of a 14" laptop.
It will be real Wii hardware, with no parts omitted.

Buyers will bring their own Wii to be modified, then pay for parts, labor, and shipping.
@selimgozel1 in the Discord will assemble the device, and ship it back, including:
- WiiTop itself, with the Wii pre-modded to boot into Linux immediately, and ArchPOWER Wii Linux installed to the internal SSD (of configurable size)
- Wii Linux boot SD (with the kernel and boot stack pre-installed)
- Special edition boxed copy of Wii Linux + ArchPOWER, including an instruction manual (in physical and electronic form), and USB stick containing the installation files and install manual PDF.
- Free technical support link (the Discord server)

## WiiTop Hardware

### Internal components
- **All components of a normal Wii, except for the case, and fan**
- Internal power supply to handle running 12V to the Wii, and whatever other voltages need to get sent to the screen and other internal components
- custom 5V DC fan and heat pipe assembly to cool the Wii in a laptop form factor
- 854x480 Screen (480p but 16:9)
- Some small battery, probably only 10-20Wh or so
- USB-C Power Delivery board to handle charging the battery
- Wii AV out (component) -> LVDS / eDP / whatever the screen uses
- the Wii's own 2 USB ports
  - port 1
    - internal USB 6-port hub
      - the WiiTop's USB Keyboard
      - USB -> SATA adapter to connect the internal storage
      - the DDR3 SODIMM -> USB storage custom chip
      - power management controller to report battery status
      - 2x 4-pin USB 2.0 internal expansion header on the board
  - port 2
    - external USB 4-port hub, connecting the 4 external ports
- SATA data and power combined cable (power routing to the internal PSU), for connecting the internal storage
- SATA SSD included, user replacable/upgradable

### External components
- 4 external USB ports - 2 on each side
- 1 external USB-C port for charging only (no data)
- All ports (except USB) that sit on the actual Wii
  - SD Card slot
  - (**possible, not guaranteed**) DVD-ROM bay
  - GameCube controller ports
  - GameCube memory card ports for USB Gecko (Gecko not included)
- Custom sensor bar (literally 2 IR LEDs) baked into the top of the screen (think like where a webcam would go)


# Changelog (dates in MM/DD/YYYY)
Rev A (9/24/2024) - initial hardware  
Rev B (9/24/2024) - updated port 1 hub to 6-port, added power reporting interface, added 2nd internal expansion header  
Rev C (9/24/2024) - Add external USB-C port for charging  
Rev D (9/24/2024) - Make it a full specification rather than just hardware description.  Add basic description of the WiiTop  
Rev E (9/24/2024) - Add dates to the chanelog while I still can remember them (the first day of development)  
