# Fab Electronics Library for KiCad

This library (should) cover all the electronics components found in the official [fab inventory](http://fab.cba.mit.edu/about/fab/inv.html). Using this library should also make it easier to share KiCad project files between Mac, Windows and Linux systems.

> **Warning!** the library is under active development. Naming of components can change overnight. Make sure to `git pull` the latest version before doing work.

## Installation

1. Clone or download this repository. You may rename the directory to `fab`.
2. Store it in a safe place such as `~/kicad/libraries` or `C:/kicad/libraries`.
3. Run KiCad or open a KiCad `.pro` file.
4. Go to "Preferences / Manage Symbol Libraries" and add `fab.lib` as symbol library.
5. Go to "Preferences / Manage Footprint Libraries" and add `fab.pretty` as footprint library.
6. Go to "Preferences / Configure Paths" and add variable named **FAB** that points to the installation directory of the fab library, such as `~/kicad/libraries/fab` or `C:/kicad/libraries/fab`. This will enable the custom 3D shapes to be found. The 3D shapes project has just started and most of them have to be populated still.

## On-Going TODO

**Check symbols and remove duplicates**  
Add symbols with names that make sense, try to follow and come up with a Fab naming convention. Every symbol entry in `fab.lib` should have a corresponding description in the `fab.dcm` file. That makes it easier for the KiCad search to look for parts. At this point try to match to [KiCad Library Convention](https://kicad-pcb.org/libraries/klc/) as much as possible. More to follow as next big step.

- [x] Resistor
- [x] Potentiometer
- [x] Capacitor
- [x] Choke coil, inductor
- [x] Diode
- [x] Transistor (MOSFET's)
- [x] H-Bridge motor drivers
- [x] Tripple H-Bridge motor drivers
- [x] Stepper motor drivers
- [x] Regulators
- [x] Charge controllers
- [x] Amplifiers
- [x] LEDs
- [x] Photodetectors
- [x] Speakers and mics
- [x] Temperature sensors
- [x] Hall-Effect sensors
- [x] Accelerometer
- [x] Pressure sensors
- [x] Op-Amp
- [x] Microcontrollers
- [x] Memory
- [x] Programmable logic FPGA chips
- [x] Radios
- [x] Crystals
- [x] Buttons and switches
- [x] Connectors
- [x] Jacks and plugs
- [x] Battery holders
- [x] USB chips and connectors
- [x] SD card socket

Next step: Create a list of parts to test against. Maybe the [Fab Electronics Inventory](https://gitlab.fabcloud.org/pub/inventory/electronics) project can be useful here.

## Contributing

Please refer to the [CONTRIBUTING](CONTRIBUTING.md) document. Run `test.py` locally before `git push`.

## License

Please refer to the [LICENSE](LICENSE) document located in this repository.
