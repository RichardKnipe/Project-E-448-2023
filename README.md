# Design and Implementation of a Battery Input Single-Phase Pure Sine Wave Inverter for Loadshedding

## Abstract

The goal of this project was to design an off-grid, single phase voltage source inverter (VSI) that can power a TV and Wi-Fi router from a battery during loadshedding. The topic was chosen not for its originality or usefulness, but because it encompasses a broad spectrum of E&E Engineering disciplines where competence can be tested, including analog electronics, power electronics, energy systems, control systems, and embedded systems, just to name a
few. The output voltage was to be kept constant for varying loads and input voltages. A transformer out of an old UPS was the reason for a rated inverter power of 193W. LTSpice was used to simulate almost every circuit in detail. A schematic and PCB were drawn up in KiCad, and was manufactured by the University. A control system was designed an simulated in Simulink, where it proved to regulate the output voltage for varying input voltages. It was to be implemented on an ESP32 microcontroller. The original goal of the project also included a solar charge controller with MPPT, but this idea was scrapped fairly late in the semester as time got less, since the amount of effort was underestimated. Since much time was spent on this scrapped part of the project initially, this left too little time for the inverter. This is why the components were ordered late, and since they also took longer than expected to arrive, the inverter was unfortunately never tested. Nevertheless, the detailed simulations and partially populated PCB should give the reader great confidence that the inverter will have a good chance of working first try.

## Presentation Video

The following YouTube video presents the project:

[![Video Title](https://img.youtube.com/vi/ruMZNLkoVRQ/0.jpg)](https://www.youtube.com/watch?v=ruMZNLkoVRQ)
