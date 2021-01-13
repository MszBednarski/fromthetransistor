#### Section 1: Intro: Cheating our way past the transistor -- 0.5 weeks
- So about those transistors -- Course overview. Describe how FPGAs are buildable using transistors, and that ICs are just collections of transistors in a nice reliable package. Understand the LUTs and stuff. Talk briefly about the theory of transistors, but all projects must build on each other so we can’t build one.
- Emulation -- Building on real hardware limits the reach of this course. Using something like Verilator will allow anyone with a computer to play.

https://en.wikipedia.org/wiki/Transistor
https://www.build-electronic-circuits.com/how-transistors-work/
##### NPN transistor:
transistor is basically as switch which can have an on or off state.
so a transistor has 3 pins a base collector and emmiter
if you apply volatage <0.7V to the base the transistor is in an OFF state
and current doesnt flow from the collector to the emmiter
if you apply voltage >0.7v to the base the transistor is in an ON state and
current flows from the collector to the emiiter
##### PNP transistor: 
Same it has base emmiter collector. If the voltage on base = emmiter -0.7 or less, the current is allowed to flow from emmiter to collector so the transistor is ON
Else if base > emmiter -0.7V the transistor is OFF and the current is not allowed to flow from the emmiter to the collector 

##### MOSFET
metal oxide silicon field effect transistor
- base building block of modern electronics used in IC's
- when high current flows through the base the positive field attracts electrons and allows the source to flow to the drain and the mosfet is on the positive field allows the electrons to flow through this field effect

##### lets do some gates with transistors
> AND GATE: A and B: connect drain of A to source of B drain of B is output
> OR GATE: A and B: connect drain of A and drain of B and source of A and source of B in parallel to a battery
> NAND GATE: A and B: have battery line to output and connect in series source drain A B out is before source connection of A //// Since there is a resistor before battery the 1/2 of the source is below the treshold to be considered on when both A and B are on
> NOR GATE: A and B: have battery line to output and connect in parallel the source drain of A B, so whenever A or B is ON the current from the battery drops.


https://en.wikipedia.org/wiki/Integrated_circuit
##### ICs are integrated circuts
they are prepacked electronic circuts for reuse

