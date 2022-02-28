# Implementation of XNOR Using 6 MOS Transistors and 28nm CMOS Technology
XNOR gate (One Bit Equality Comparator) is designed using 28nm CMOS technology by using Synopsys Custom Compiler


# Table of Content 
- ABSTRACT 
- INTRODUCTION
- TOOLS USED
- XNOR CIRCUIT DESIGN
- NETLIST
- ACKNOWLEDGEMENT 
- REFERENCE 


## ABSTRACT

XNOR is a Hybrid gate which has OR, AND and NOT operation done to the inputs. XNOR gate is also called as equivalance gate because of the operation gives logic high when inputs are same and logic low when inputs are opposite. This is also the reason why XNOR is used as one bit equality comparator. XNOR is used for various applications like Pseudo Random number generator, Equality comparator, Correlation and sequence detection etc. Here a XNOR is designed using 28nm CMOS technology by using Synopsys Custom Compiler.

# INTRODUCTION

In the Figure below, we have achieved XNOR operation only by using 3 NMOS and 3 PMOS transistors. The circuit consists of 2 CMOS inverters and 2 MOS pass gate configuration. By clever logic hack we have achieved XNOR logic using less number of transistors.

![image](https://github.com/rahul-hebbar/XNOR_gate_using_synopsys/blob/main/images/xnor.png)

When both the inputs given are same, we get logic high as output indicating us that both the inputs are of same logic. When both inputs are of different logics, we get a logic low.

# TOOL USED

- Synopsys Custom Compiler:  The Synopsys Custom Compiler™ design environment is a modern solution for full-custom analog, custom digital, and mixed-signal IC design. As the heart of the Synopsys Custom Design Platform, Custom Compiler provides design entry, simulation management and analysis, and custom layout editing features. This tool was used to design the circuit on a transistor level.

- Synopsys Primewave:  PrimeWave™ Design Environment is a comprehensive and flexible environment for simulation setup and analysis of analog, RF, mixed-signal design, custom-digital and memory designs within the Synopsys Custom Design Platform. This tool helped in various types of simulations of the above designed circuit.

- Synopsys 28nm PDK:  The Synopsys 28nm Process Design Kit(PDK) was used in creation and simulation of the above designed circuit.

# XNOR CIRCUIT DESIGN

The CMOS design for XNOR is shown in fig. 

![image](https://github.com/rahul-hebbar/XNOR_gate_using_synopsys/blob/main/images/circuit.png)

- SCHEMATIC

![image](https://github.com/rahul-hebbar/XNOR_gate_using_synopsys/blob/main/images/schematic.png)

                                                                                                                                                                                                                                                                                                                                                                            
- SYMBOL

![image](https://github.com/rahul-hebbar/XNOR_gate_using_synopsys/blob/main/images/symbol.png)                                                                                                                                                                                                                                                                                                                                                                               

- TESTBENCH SYMBOL

![image](https://github.com/rahul-hebbar/XNOR_gate_using_synopsys/blob/main/images/sim_schem.png)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                
- PRIMEWAVE WINDOW

![image](https://github.com/rahul-hebbar/XNOR_gate_using_synopsys/blob/main/images/testsuit_pathway.png)                                                                                                                                                                                                                                                                                                                                                                                                                                                        
- TESTBENCH WAVEFORM

![image](https://github.com/rahul-hebbar/XNOR_gate_using_synopsys/blob/main/images/waveform.png)                                            

# NETLIST
The netlist of the above circuit has also been uploaded to the github repo with the file name - netlist.txt  

# AUTHOR
P R RAHUL HEBBAR, MTech VLSI and Embedded Systems , Defence Institute of Advanced Technology, Pune, Maharashtra

# ACKNOWLEDGEMENT 

- Kunal Ghosh, Co-founder, VSD Corp. Pvt. Ltd.
- Synopsys, India
- VLSI System Design(VSD) Corporation Private Limited India
- Indian Institute of Technology, Hyderabad 
- Cloud Based Analog IC Design Hackathon
- Sameer Durgoji, NIT Karnataka
- Chinmay panda, IIT Hyderabad

# REFERENCES

- Cristiano Calligaro,(2008) Design of a rad-hard library of digital cells
for space applications.
- Fig 1. Courtesy of electronics-tutorial.net, https://www.electronics-tutorial.net/digital-logic-gates/xnor-gate/

