[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7118008.svg)](https://doi.org/10.5281/zenodo.7118008)

# Project Heptapod

*I2C and RS-485 bus breakout boards by [Northern Widget LLC](https://www.northernwidget.com)*

![Heptapod I2C Bus Breakout](Documentation/images/Heptapod_BusBreakout_I2C_2025.jpg)

## Overview

Project Heptapod is a family of small breakout boards designed to connect multiple sensors to a data logger or microcontroller. The name comes from *hepta* (Greek: seven), reflecting the board's ability to fan out a single bus connection to seven sensor ports.

## Boards

### BusBreakout\_I2C

A passive I2C bus breakout that splits one upstream I2C connection (SCL, SDA, VCC, GND) into seven downstream screw-terminal ports. Designed for use with the [Northern Widget Margay](https://github.com/NorthernWidget/Project-Margay) or any I2C-capable data logger.

### Switched\_I2C

An I2C breakout with software-switchable power to each port, allowing the host controller to selectively power sensors and reduce quiescent current in low-power deployments.

### RS485\_Breakout

An RS-485 bus breakout for multi-drop sensor networks over long cable runs.

## License

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.
