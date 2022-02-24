# Half_Adder_analog_design
This repository presents the design of Half Adder implemented using Synopsis Custom Compiler on 28nm CMOS Technology.

### Table of Contents
 - [Introduction](#introduction)
 - [Reference Circuit Diagram](#reference-circuit-diagram)
 - [Reference Circuit Waveform](#reference-circuit-waveform)
 - [Tools Used](#tools-used)
 - [Schematics and Simulations:](#schematics-and-simulations)
 - [Netlist of the Circuit:](#netlist-of-the-circuit)
 - [Author:](#author)
 - [Acknowledgements:](#acknowledgements)
 - [References:](#references)
 
## Introduction
Half adder is a digital combinational circuit that executes addition of two single bit binary numbers and generates two outputs i.e., a sum bit (S) and carry bit (C). If A and B are taken as primary input bits, then sum bit (S) is obtained by X-ORing of input bits A and B and the carry bit (C) is obtained by ANDing of input bits A and B. Block diagram, logic diagram and truth table of half adder are shown in Figure 1 and Table 1 respectively. The Boolean expression of half adder[2] is given by: 
S= A⊕ B and C=A.B 


![HA](https://user-images.githubusercontent.com/100190726/155269489-a46fd3d3-1d0f-40b4-bcae-6450b93dc745.JPG)

Fig. 1: Block Diagram of Half Adder and Logic Diagram of Half Adder

![HA_TT](https://user-images.githubusercontent.com/100190726/155269581-422270c2-d13a-41a4-bf47-061f11464790.JPG)


Table 1: Truth Table of Half Adder. Procedure for Paper Submission
## Reference Circuit Diagram
Complementary Metal Oxide Semiconductor (CMOS) logic[1] deploys symmetric number of both types of MOSFETs, i.e., pMOS and nMOS. This leads to better performance of any logic circuit since nMOS is strong ‘0’ device and pMOS is strong ‘1’device. Thus, CMOS provides complete ‘1’ and complete ‘0’ logics at the output without any distortion. Half Adder using CMOS modeled using 12 transistors as shown in Figure 3.


![HA_ckt](https://user-images.githubusercontent.com/100190726/155269685-35736a80-902c-4a0a-a1a4-cb42d4830b48.JPG)

 
Figure 3. Half Adder Using CMOS Logic.

## Reference Circuit Waveform

 ![image](https://user-images.githubusercontent.com/100190726/155500159-a895317c-c1b6-4a48-833c-3c5fcbabc9be.png)



## Tools Used:
• Synopsys Custom Compiler:
 The Synopsys Custom Compiler™ design environment is a modern solution for full-custom analog, custom digital, and mixed-signal IC design. As the heart of the Synopsys Custom Design Platform, Custom Compiler provides design entry, simulation management and analysis, and custom layout editing features. This tool was used to design the circuit on a transistor level.

• Synopsys Primewave:
 PrimeWave™ Design Environment is a comprehensive and flexible environment for simulation setup and analysis of analog, RF, mixed-signal design, custom-digital and memory designs within the Synopsys Custom Design Platform. This tool helped in various types of simulations of the above designed circuit.

• Synopsys 28nm PDK:
 The Synopsys 28nm Process Design Kit(PDK) was used in creation and simulation of the above designed circuit.
 
 ## Schematics and Simulations:
 ### Schematics:
 ### Half Adder
 Initially Schematic of the Half Adder cell was implemented and converted into a symbol so that it could be used directly as delay cell from the library.
 
 
 ![ha_sch](https://user-images.githubusercontent.com/100190726/155284404-ad60f01a-13b8-4640-8914-06020052f87e.JPG)

 
 Fig. 4: Half Adder Cell Schematic
 
 
 ![ha_sym](https://user-images.githubusercontent.com/100190726/155284499-95dbccd7-0036-4988-9244-3bf942ebfa5e.JPG)

 Fig. 5: Half Adder Cell Symbol
 
 ### Parameters set for Voltage Source for Input A
 
 ![A](https://user-images.githubusercontent.com/100190726/155505423-33d7dd09-e86e-4ed5-9063-c6e9071985af.JPG)


 
 
 
 ### Parameters set for Voltage Source for Input B
 
 
 ![B](https://user-images.githubusercontent.com/100190726/155505312-5892520a-c083-4d9a-a4ba-a13dd4aa468e.JPG)

 

 
 
 ![ha_test](https://user-images.githubusercontent.com/100190726/155284515-8187e068-cbd4-4fc6-bf4c-4d0ab1ffc863.JPG)

 Fig. 6: Half Adder Test Circuit 
 
  ### Transient Settings
 
 ### Simulations:
 ### Transient Analysis:
After creating and saving the schematic go to 'Tools' and open 'Primewave' to start the simulation. In the Primewave select the 'model file' i.e the '28nm PDK's .lib file presentin the HSPICE folder. After this select the 'tran' analysis in the analysis window and give the 'Start', 'Stop', and 'Step Size' parameters and save it. Then add the outputs which needs to be plotted by selecting the nets on the schematic.

![transient](https://user-images.githubusercontent.com/100190726/155507012-b7369b24-be78-401d-aae3-884e000e7ce0.JPG)


Then go to 'Simulations -> Netlist and Run' to generate a netlist and run the simulation to get the below output.

![ha_wave](https://user-images.githubusercontent.com/100190726/155284548-f95e65f7-0e13-40d9-ba06-64a3aa05d801.JPG)

Fig. 7: Half Adder Transient Analysis


## Netlist of the Circuit:
Refer to the netlist of the circuit here:[netlist.txt](https://github.com/swati-sgm/Half_Adder_analog_design/files/8129767/netlist.txt)



## Author:
Swati Mavinkattimath, Assistant Professor, KLE Dr. M S Sheshgiri College of Engineering and Technology Belagavi- 590008

## Acknowledgements:
- [Cloud Based Analog IC Design Hackathon](https://www.iith.ac.in/events/2022/02/15/Cloud-Based-Analog-IC-Design-Hackathon/)
- [Synopsys India](https://www.synopsys.com/)
- [VLSI System Design (VSD) Corp. Pvt. Ltd India](https://www.vlsisystemdesign.com/)
- Kunal Ghosh, Co-founder, VSD Corp. Pvt. Ltd.
- Chinmay panda, IIT Hyderabad
- Sameer Durgoji, NIT Karnataka
## References:
- Rituraj Yadav, Ashish Sura, Sunita Dahiya, “HALF ADDER DESIGN USING VARIOUS TECHNOLOGIES AND COMPARISON OF VARIOUS PARAMETER PERFORMANCE” International Journal of Engineering Applied Sciences and Technology, 2021 Vol. 6, Issue 2, ISSN No. 2455-2143, Pages 95-100 
- Rajput, Anju & Dua, Tripti & Kumawat, Renu & Srinivasulu, Prof. Avireni. (2020). Half Adder Using Different Design Styles: A Review on Comparative Study. 7. 26-32.
- Murugesan, Sivakumar & Sundaramurthy, Omkumar. (2017). Implementation of Area & Power Optimized VLSI Circuits Using Logic Techniques. IOSR Journal of VLSI and Signal Processing (IOSR-JVSP). 7. 15-23. 
