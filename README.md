# Half_Adder_analog_design
This repository presents the design of Half Adder implemented using Synopsis Custom Compiler on 28nm CMOS Technology.

# Table of Contents

# Introduction
Half adder is a digital combinational circuit that executes addition of two single bit binary numbers and generates two outputs i.e., a sum bit (S) and carry bit (C). If A and B are taken as primary input bits, then sum bit (S) is obtained by X-ORing of input bits A and B and the carry bit (C) is obtained by ANDing of input bits A and B. Block diagram, logic diagram and truth table of half adder are shown in Figure 1 and Table 1 respectively. The Boolean expression of half adder[2] is given by: 
S= A⊕ B and C=A.B 


![HA](https://user-images.githubusercontent.com/100190726/155269489-a46fd3d3-1d0f-40b4-bcae-6450b93dc745.JPG)

Fig. 1: Block Diagram of Half Adder and Logic Diagram of Half Adder

![HA_TT](https://user-images.githubusercontent.com/100190726/155269581-422270c2-d13a-41a4-bf47-061f11464790.JPG)


Table 1: Truth Table of Half Adder. Procedure for Paper Submission
# HALF ADDER CIRCUIT DESIGN
Complementary Metal Oxide Semiconductor (CMOS) logic[1] deploys symmetric number of both types of MOSFETs, i.e., pMOS and nMOS. This leads to better performance of any logic circuit since nMOS is strong ‘0’ device and pMOS is strong ‘1’device. Thus, CMOS provides complete ‘1’ and complete ‘0’ logics at the output without any distortion. Half Adder using CMOS modeled using 12 transistors as shown in Figure 3.


![HA_ckt](https://user-images.githubusercontent.com/100190726/155269685-35736a80-902c-4a0a-a1a4-cb42d4830b48.JPG)

 
Figure 3. Half Adder Using CMOS Logic.
