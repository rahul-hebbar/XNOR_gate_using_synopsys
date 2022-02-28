# Implementation of D-Flip Flop Using 28nm CMOS Technology
The D flip flop is designed using 28nm CMOS technology by using Synopsys Custom Compiler


# Table of Content 
- ABSTRACT 
- INTRODUCTION
- TOOLS USED
- D FLIP FLOP CIRCUIT DESIGN
- CMOS NAND GATE
- CMOS INVERTER
- CMOS D FLIP FLOP
- SETUP & HOLD TIME
- POWER CALCULATION 
- SIMULATION RESULT
- NETLIST
- ACKNOWLEDGEMENT 
- REFERENCE 


## ABSTRACT

Flip Flops are basic building blocks of digital electronic circuits used in communications, Computers, and many circuits and have stable states that store binary data. The stored data can be changed by applying varying inputs. In this paper, the D flip flop is designed using 28nm CMOS technology by using Synopsys Custom Compiler.

# INTRODUCTION

A D (or Delay) Flip Flop shown in Figure is a digital electronic circuit used to delay the change of state of its output signal (Q) until the next rising edge of a clock timing input signal occurs. Flip Flop is a sequential circuit, which is used to store a single bit of information. Flip-Flop is an edgetriggered sequential block. The major applications of D flipflop are to introduce delay in timing circuit, as a buffer, sampling data at specific intervals.

![image](https://user-images.githubusercontent.com/70645320/155837784-3cf8107f-c83f-493f-ae18-8bc76de1c2d8.png)    ![image](https://user-images.githubusercontent.com/70645320/155837790-f437d631-d031-48c9-a040-75542af2b22b.png)

When the D input is provided to the Flip Flop, the circuit check for the clock signal is the signal of the clock is high (for level triggered d flip-flop) then with every clock pulse, the input D propagates to the output Q. For edge-triggered flipflop, the circuit check for the transition of clock pulse according to which the flip Flop propagates the input to the output; edge-triggered can be positive edge-triggered or negative triggered. Positive edge-triggered D flip-flop changes its output according to input with every transition of the clock pulse from 0 to 1. As for the negative edge-triggered D, flip-flop changes its output according to input with every transition of the clock pulse from 1 to 0.

# TOOL USED

- Synopsys Custom Compiler:  The Synopsys Custom Compiler™ design environment is a modern solution for full-custom analog, custom digital, and mixed-signal IC design. As the heart of the Synopsys Custom Design Platform, Custom Compiler provides design entry, simulation management and analysis, and custom layout editing features. This tool was used to design the circuit on a transistor level.

- Synopsys Primewave:  PrimeWave™ Design Environment is a comprehensive and flexible environment for simulation setup and analysis of analog, RF, mixed-signal design, custom-digital and memory designs within the Synopsys Custom Design Platform. This tool helped in various types of simulations of the above designed circuit.

- Synopsys 28nm PDK:  The Synopsys 28nm Process Design Kit(PDK) was used in creation and simulation of the above designed circuit.

# D FLIP FLOP CIRCUIT DESIGN

the D FF can be designed using NOR or NAND gates as shown in fig. The D input is sampled during the occurrence of a clock pulse. If it is 1, the flip-flop is switched to the set state (unless it was already set). If it is 0, the flip-flop switches to the clear state. ). The Circuit in fig is a masterslave D flip-flop. A D flip flop takes only a single input, the D (data) input. The master-slave configuration has the advantage of being edge-triggered, making it easier to use in larger circuits, since the inputs to a flip-flop often depend on the state of its output. The circuit consists of two D flip-flops connected. When the clock is high, the D input is stored in the first latch, but the second latch cannot change its state. When the clock is low, the first latch's output is stored in the second latch, but the first latch cannot change its state. The Design is implemented using Synopsys Custom Compiler in 28 nm CMOS technology.

![image](https://user-images.githubusercontent.com/70645320/155837958-ba29461d-4e27-4257-9917-a46742eaabd7.png)

                                                                                                                                                                                                                                                                                                                                                                    

# CMOS NAND GATE
The CMOS design for the NAND is shown in fig. Here we have used 2 diffrent NAND gate. In NAND_2X W/L ratio for PMOS is 2 and NMOS is 1, in NAND_1X W/L ratio for PMOS is 1 and NMOS is 1.

![image](https://user-images.githubusercontent.com/70645320/155849735-42887eef-69a4-4ea2-a6e8-1b4dbc9b9c14.png)
![image](https://user-images.githubusercontent.com/70645320/155849739-13bafc32-c7b0-4483-9097-89380e561bbc.png)

                                                                                                                                                                                                                                                                                                                                                                 

# CMOS NAND_1X GATE 
- SCHEMATIC

![image](https://user-images.githubusercontent.com/70645320/155850129-85a12e9c-9169-4d7d-835c-688be713ee1d.png)

                                                                                                                                                                                                                                                                                                                                                                            
- SYMBOL

![image](https://user-images.githubusercontent.com/70645320/155850166-17e48606-1f89-4dbf-9fa2-80026f72df1d.png)                                                                                                                                                                                                                                                                                                                                                                               

- TESTBENCH SYMBOL

![image](https://user-images.githubusercontent.com/70645320/155850261-fb896b6a-117d-458d-bfcb-82ecabbed77e.png)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                
- PRIMEWAVE WINDOW

![image](https://user-images.githubusercontent.com/70645320/155850309-fc5c3f6c-f9ca-4194-ad4c-ad019951ce00.png)                                                                                                                                                                                                                                                                                                                                                                                                                                                        
- TESTBENCH WAVEFORM

![image](https://user-images.githubusercontent.com/70645320/155850354-6eb6664f-95c0-4bcc-a7f9-9014ec92b198.png)                                                                                                                                                                                                                                                  
# CMOS NAND_2X GATE 

- SCHEMATIC
![image](https://user-images.githubusercontent.com/70645320/155850638-1ce89522-f48b-4d48-a95e-e8645c0439d2.png)


- SYMBOL
![image](https://user-images.githubusercontent.com/70645320/155850646-cb679f54-1799-42f9-a805-64192a6ae184.png)



- TESTBENCH SYMBOL
![image](https://user-images.githubusercontent.com/70645320/155850656-5101b75d-c9c6-481d-8813-469891521e18.png)



- PRIMEWAVE WINDOW
![image](https://user-images.githubusercontent.com/70645320/155850665-d08017aa-080b-4c88-ab3a-2465e0a0431a.png)



- TESTBENCH WAVEFORM
![image](https://user-images.githubusercontent.com/70645320/155850671-881ca845-76d2-4e55-924c-b9d3868dae3f.png)





# CMOS INVERTER GATE
The CMOS design for the Inverter is shown in fig.

![image](https://user-images.githubusercontent.com/70645320/155850021-7845e794-bbfe-49fd-835a-991e2c7a09fa.png)

- SCHEMATIC

![image](https://user-images.githubusercontent.com/70645320/155850808-d456da3e-3720-42a2-a0fe-67cdafe37807.png)

- SYMBOL

![image](https://user-images.githubusercontent.com/70645320/155850816-6e2b4107-cbcb-4441-b1f0-923e4efaf41d.png)



- TESTBENCH SYMBOL
![image](https://user-images.githubusercontent.com/70645320/155850831-39c5474a-db91-4ab3-8da5-6546b819730d.png)



- PRIMEWAVE WINDOW

![image](https://user-images.githubusercontent.com/70645320/155850839-5b2822db-8415-4d7c-8690-09fab6655fa3.png)


- TESTBENCH WAVEFORM

![image](https://user-images.githubusercontent.com/70645320/155850847-e63358f7-2754-4c6e-baa0-214a0be3518f.png)

# CMOS D FLIP FLOP

-  SCHEMATIC

![image](https://user-images.githubusercontent.com/70645320/155851288-65d66977-381e-4b01-b6e9-e611086f1a06.png)


-  SYMBOL

![image](https://user-images.githubusercontent.com/70645320/155851294-066a3df3-bd8d-4fd2-ba8d-cc27c26453ec.png)

1. INPUT = VPULSE WAVE 
-  TESTBENCH SYMBOL

![image](https://user-images.githubusercontent.com/70645320/155851484-e33cb9af-7795-489a-92d9-a4f0abae6c08.png)


-  PRIMEWAVE WINDOW

![image](https://user-images.githubusercontent.com/70645320/155851499-66a9d6d6-9529-449f-b27b-fabc4c88a927.png)

-  TESTBENCH WAVEFORM

![image](https://user-images.githubusercontent.com/70645320/155851508-0cab518e-beca-4490-92bc-bcfae1ed456e.png)


2. INPUT = VPWL WAVE
-  TESTBENCH SYMBOL

![image](https://user-images.githubusercontent.com/70645320/155851658-2a260f9c-950d-451b-9979-0ac6ed3a88bf.png)

-  PRIMEWAVE WINDOW


![image](https://user-images.githubusercontent.com/70645320/155851912-bf242eee-bc9f-47e3-a91d-8081ab920d83.png)


-  TESTBENCH WAVEFORM

![image](https://user-images.githubusercontent.com/70645320/155851932-370bfd4c-d1fe-4691-98ff-b040905ce4d6.png)

# SETUP TIME & HOLD TIME

- Setup time  

Minimum time requires for which the data should be stable before the active edge of the clock. Tcq is clock to output delay. Tdc is data to active edge difference. 


- Setup Rise time 

To calculate the setup rise time the output should be logic 0. So when the active edge comes the output becomes logic 1, for given high input. When we shift the data from left to right across the active edge of the clock, if data is far from the active edge Tcq(Clock to output delay) is stable. When data comes near to the active edge of the clock, the Tcq will start increasing after some time it fails. When data is far from the active edge the Tcq is said to be base delay. So when Tcq = 110% of base delay, At that time the value of Tdc is called setup rise time.

- PRIMEWAVE PARAMETERS

Here we have varried the input voltate coordinate t1 from 4.8n to 5.1n sec.
![image](https://user-images.githubusercontent.com/70645320/155858521-ffc3da02-9240-4219-bbd0-7719892f39db.png)

- TESTBENCH RESULTS

From the results we have observed the tcq is 119.5p sec.
Then for 110% of tcq is 131.45p sec. 
![image](https://user-images.githubusercontent.com/70645320/155858638-975f719b-af83-4e90-91a5-9b36ed6dfac5.png)


- PRIMEWAVE PARAMETERS
Here we have varried the input voltage coordinate t1 from 5.080n to 5.085n sec.
![image](https://user-images.githubusercontent.com/70645320/155858722-58bd8fc0-ff80-4d2d-92ff-1fe717a6cc50.png)

- TESTBENCH RESULTS

From the testbench result we can observe that for tcq =131.45p sec the calculated tcd= -42.1p sec
Calculated Set up time = -42.1p sec
![image](https://user-images.githubusercontent.com/70645320/155858746-9da3f438-cce8-419d-95b6-d69a752ad55a.png)

- TESTBENCH WAVEFORM

![image](https://user-images.githubusercontent.com/70645320/155858684-4ef99d0c-94a9-43eb-b2ed-0634dcfd9884.png)



- Hold time 

Minimum time required for which the data should be stable after the active edge of the clock.


- Hold Rise time
 
To calculate the hold rise time the output should be logic 1. So when the active edge comes the output becomes logic 0, for given high input.
When we shift the data from right to left across the active edge of the clock, if data is far from the active edge Tcq(Clock to output delay) is stable. When data comes near to the active edge of the clock, the Tcq will start increasing after some time it fails. When data is far from the active edge the Tcq is said to be base delay. So when Tcq = 110% of base delay at that time the value of Tdc is called hold rise time.

- PRIMEWAVE PARAMETERS


Here we have varried the input voltate coordinate t2 from 5.1n to 4.8n sec. We can see the violation of tcq from the graph. After t2= 5.085n sec the output is reaching the meta unstable state.
![image](https://user-images.githubusercontent.com/70645320/155858949-b5dfc9a2-1f3c-400c-96ad-acad086bac4f.png)

- TESTBENCH RESULTS


From the results we have observed the tcq is 136.7p sec.
Then for 110% of tcq is 150.37p sec.
 ![image](https://user-images.githubusercontent.com/70645320/155859078-8e10dfe9-7643-4ccb-a727-bce4289e8367.png)


- PRIMEWAVE PARAMETERS

Here we have varried the input voltage coordinate t2 from 5.086n to 5.085n sec.
![image](https://user-images.githubusercontent.com/70645320/155859082-64b6eb51-aa5b-44a6-b541-54c734d0e3f2.png)

- TESTBENCH RESULTS


From the testbench result we can observe that for tcq =150.37p sec the calculated tcd= -39.74p sec
Calculated Hold time = -39.74p sec

![image](https://user-images.githubusercontent.com/70645320/155859154-a6b5d159-869b-4ba4-a179-7dcc61b153b1.png)


- TESTBENCH WAVEFORM


![image](https://user-images.githubusercontent.com/70645320/155859246-f7b6efdd-5ebd-4abd-80b1-e5560219380c.png)



# POWER CALCULATION 

- Steps to calculate the Avg Current

 1. Take Vdd node Current from the output option(Select from the Design). I have named it as current_ff
 2. Open the calculator from output option and select mean filter. 
 3. Give Required values (current_ff, 200ps, 4.2n). We need to give the 3rd value as integer multiple of time period thats why i took it for 4 cycles(you can take any number of cycles)
 4. Now netlist and run the simulation
 5. Open viewer from the results option
 6. We can see the Avg Current value is 1.46269u amp

- PRIMEWAVE PARAMETERS


The value of average current at Node vdd is calucalted for 1 GHZ clock frequency.
![image](https://user-images.githubusercontent.com/70645320/155859450-d4d06ecb-c9b3-4e5e-b479-46ead44332a1.png)


- TESTBENCH RESULTS


The value of average current is 1.46269u amp.
![image](https://user-images.githubusercontent.com/70645320/155859519-78cdc96f-284b-4e9e-b542-806ec057c41a.png)


- TESTBENCH WAVEFORM


![image](https://user-images.githubusercontent.com/70645320/155859568-360add16-d150-4015-b1d4-932ed5b07ff6.png)



# SIMULATION RESULT

- Set up time = -42.1p sec
- Hold time = -39.74p sec
- Average Current = 1.46269u amp

# AUTHOR
Sonu Agrawal, MTech Embedded Systems, Vellore Institute of technology, Vellore, Tamil Nadu

# ACKNOWLEDGEMENT 

- Kunal Ghosh, Co-founder, VSD Corp. Pvt. Ltd.
- Synopsys, India
- VLSI System Design(VSD) Corporation Private Limited India
- Indian Institute of Technology, Hyderabad 
- Cloud Based Analog IC Design Hackathon
- Sameer Durgoji, NIT Karnataka
- Chinmay panda, IIT Hyderabad

# REFERENCES

- Seelam Vasavi Sai Viswanada Prabhu Deva Kumar et al.2017, “Implementation of Low Power D-Flipflop Using 45nm Cmos Technology,” Int J Recent Sci Res. 8(6), pp. 17729-17732.
- Praveen Kumar, Jasbir Kaur, “Design of Various D Latch And Flip- Flop Using 180nm Technology,” 2007 IJEEE, vol 9.
- Mohamedsulaiman, S. & Be, Jaison & Bennet, M. & Rahman, S. & Priyan, V. & Raj, J. & Kumar, V.. (2019). “Design and implementation of sequential circuit based on low power using 45nm technology,”.International Journal of Recent Technology and Engineering. 7. 212-218.

