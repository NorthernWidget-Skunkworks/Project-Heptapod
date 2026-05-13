[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7118007.svg)](https://doi.org/10.5281/zenodo.7118007)

# Project Ophiura

*I2C and RS-485 bus breakout boards by [Northern Widget LLC](https://www.northernwidget.com)*

![Ophiura I2C Bus Breakout](Documentation/images/Heptapod_BusBreakout_I2C_2025.jpg)

## Namesake

![Ophiura albida brittle star](Documentation/images/Ophiura_albida_aboral.jpg)

***Ophiura albida*, a brittle star.** *Photo by Andrea Bonifazi, [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/).*

*Ophiura* (pronounced "oh-FYOO-rah"; from Greek *ophioura*, "snake-tailed") is a genus of brittle stars — marine invertebrates related to sea stars but built for sensing and coordinated movement. When a brittle star locomotes, one arm leads as a sensory probe while the other four row in coordinated response. Crucially, all four trailing arms continuously send proprioceptive feedback back to the central disc, which integrates and adjusts. The result is a true bidirectional hub: signals flow outward from one to four, and inward from four back to one.

This maps directly onto I2C: one upstream connection carries clock and commands outward to sensors, while sensors pull the data line back to return their readings. Project Ophiura is not a splitter — it is a hub.

## Overview

Project Ophiura is a family of compact breakout boards for distributing bus connections. The most widely used board is the **BusBreakout\_I2C**, which connects a single upstream I2C connection (SCL, SDA, VCC, GND) to four independent downstream screw-terminal ports — making it easy to wire multiple sensors to one data logger or microcontroller without soldering.

Because the board is simply a passive connection hub, it can also serve as a general-purpose wire distribution point for any four-wire signal.

## [BusBreakout\_I2C](BusBreakout_I2C/)

One upstream I2C connection (typically a 4-pin header from a data logger such as the [Northern Widget Margay](https://github.com/NorthernWidget/Project-Margay)) fans out to four downstream screw-terminal ports. Each port carries SCL, SDA, VCC, and GND. No active components — plug in, tighten screws, done.

![Ophiura wired with sensors in lab](Documentation/images/HeptapodInLab_wired_closeup_2019-11-26_17.41.30.jpg)

A **Mini** variant ([BusBreakout\_I2C\_Mini](BusBreakout_I2C_Mini/)) is also available with a smaller footprint for space-constrained installations.

## Other Boards

[**Switched\_I2C**](Switched_I2C/) — I2C breakout with software-switchable power per port, allowing the host to selectively energize sensors and minimize quiescent current in low-power deployments.

[**RS485\_Breakout**](RS485_Breakout/) — RS-485 bus breakout for multi-drop sensor networks over long cable runs.

## License

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.
