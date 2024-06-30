# Design and Implementation of a Battery Input Single-Phase Pure Sine Wave Inverter for Loadshedding

## Lessons from the Real World

<img src="images/.jpeg" width="500" />

This topic was chosen for its relevance to the loadshedding era, and it covered a broad spectrum of E&E engineering disciplines where competence could be tested, such as analogue electronics, power electronics, energy systems, control systems, and embedded systems. The inverter was successfully designed to keep the output voltage of 230V constant for varying loads up to 193W, and varying input voltages due to the fluctuation of the 24V battery’s voltage.

However, this project failed for multiple reasons, all boiling down to a lack of experience with a real-world project, and perfectionism. Wanting to do what interested me the most, I chose a self-proposed topic that did not align well with my supervisor’s field of expertise, instead of choosing one of the three options he gave me. The result was that I seriously underestimated the time it would take to design and build both an MPPT solar charge controller and an inverter, which I insisted on making pure sine wave because I wanted to make a good quality product. The realisation came too late, forcing me to scrap all my charge controller work and to focus solely on the inverter.

Furthermore, since it was my first time ever designing a PCB and ordering components online, I had no idea I had to leave multiple weeks for hardware debugging and especially supply chain issues, which was the university’s problem up until then. The result was that I spent most of my time on the design. I kept optimising it until I thought it was perfect before ordering components, because I did not want to make any mistakes or waste money. Long story short, most of my components arrived after the report deadline, and all went down-hill from there… The hardest part to accept was when my supervisor mentioned afterwards that, had it been the initial goal, my design's level of detail was sufficient to be considered a final-year project on its own.

A good example of my ignorance in the real-world scenario was that I thought power ratings of components were rated for peak power, where they are instead rated for average power. This is the reason for the oversized resistors, diodes, inductors, and heat sinks, which wasted a lot of money. There were also some serious mistakes with the PCB which could have been resolved had I left more time for such issues. I did not consider the fact that the university’s PCB manufacturing service did not plate vias through, since it was a cutting machine. This left me with the impossible task of making a solid soldering connection for the legs of the inductors in the tiny space in-between them and the PCB, and since the inductors were so large the solder would not melt against the legs. Another crucial mistake was choosing the wrong footprint for the MOSFET driver IC, opting for tiny pads instead of pins. This forced me to consult a soldering specialist to connect intricate wires from each PCB pad to each pad on the IC.

All in all, I learned the hard way that making mistakes is inevitable and the best way to learn. It's crucial to consider practical limitations and to not over-engineer. I learned from my father that perfectionism is one of the sins in Jonathan Rowson’s book, The Seven Deadly Chess Sins: “Self-belief is not about thinking you will never go wrong, but rather knowing you can and will go wrong, but that these mistakes don’t define you.”

<img src="images/.jpeg" width="500" />    (put sparse PCB top and bottom here)

## Dedication until the End

Although my report was already submitted, I did what I could to be prepared for the oral presentation, which also contributed to the final mark, albeit only slightly. I ended up receiving almost all the components and soldered them onto the PCB, because I reckoned that a working inverter could potentially persuade my examiner. I succeeded in getting the low-side MOSFETs of the H-bridge to switch the 24V batter voltage as designed (see Figure 1), but since the gate drivers of the high-side MOSFETs and their bootstrap circuits did not function properly and I had no spare gate drivers to replace one of them that was definitely broken, this made the inverter useless. Nevertheless, I learned some valuable lessons, such as always making sure you have enough components when time is critical, and that ample time have to be allocated for potential hardware debugging.

<img src="images/.jpeg" width="500" />      (show an image of the fully populated PCB)

### Some Final Results



<img src="images/.jpeg" width="500" />


## Presentation Video

The following YouTube video presents the project and illustrates the thorough design:

[![Video Title](https://img.youtube.com/vi/ruMZNLkoVRQ/0.jpg)](https://www.youtube.com/watch?v=ruMZNLkoVRQ)
