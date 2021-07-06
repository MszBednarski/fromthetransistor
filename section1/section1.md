#### Section 1: Intro: Cheating our way past the transistor -- 0.5 weeks
- So about those transistors -- Course overview. Describe how FPGAs are buildable using transistors, and that ICs are just collections of transistors in a nice reliable package. Understand the LUTs and stuff. Talk briefly about the theory of transistors, but all projects must build on each other so we can’t build one.
- Emulation -- Building on real hardware limits the reach of this course. Using something like Verilator will allow anyone with a computer to play.

https://en.wikipedia.org/wiki/Transistor
https://www.build-electronic-circuits.com/how-transistors-work/
# NPN transistor
transistor is basically as switch which can have an on or off state.
so a transistor has 3 pins a base collector and emmiter
if you apply volatage <0.7V to the base the transistor is in an OFF state
and current doesnt flow from the collector to the emmiter
if you apply voltage >0.7v to the base the transistor is in an ON state and
current flows from the collector to the emiiter
# PNP transistor
Same it has base emmiter collector. If the voltage on base = emmiter -0.7 or less, the current is allowed to flow from emmiter to collector so the transistor is ON
Else if base > emmiter -0.7V the transistor is OFF and the current is not allowed to flow from the emmiter to the collector 

# MOSFET
metal oxide silicon field effect transistor
- base building block of modern electronics used in IC's
- when high current flows through the base the positive field attracts electrons and allows the source to flow to the drain and the mosfet is on the positive field allows the electrons to flow through this field effect

## lets do some gates with transistors
AND GATE: A and B: connect the emitter of A to the collector of B. 
Bam done, the inputs are the bases of A and B, the output is the emitter of B

OR GATE: A and B: connect the transistors in parallel to the output, done

NAND GATE: do the same thing like AND gate but move the output to the collector of A thus if both A and B are activated the voltage on output is too low

NOR GATE: do the same thing as the OR gate but move the output to the collector of A and B

NOR GATE (single transistor): move the A B inputs to be in parallel at the base of the single transistor, output at the collector, bam done. 

http://hyperphysics.phy-astr.gsu.edu/hbase/Electronic/trangate.html

https://en.wikipedia.org/wiki/Integrated_circuit

## ICs are integrated circuts
they are prepacked electronic circuts for reuse
mosfet is the used type of transistor nowadays
manufactured by the means of photolitgraphy etc
shining light on wafers of silicon to make circuts designed in some software

## FPGA
https://en.wikipedia.org/wiki/Field-programmable_gate_array
FPGAs are ICs that are programmable at any time

LUTs are programmable logic blocks which are basically lookup tables that let us change the output for any input and are a big part of FPGAs