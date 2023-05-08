Download Link: https://assignmentchef.com/product/solved-ve270-assignment-3-design-of-a-simple-alu
<br>
To design a simple datapath using combinational building blocks in Xilinx ISE, and to implement the circuit in an FPGA chip.

2. Design Specification

The purpose of datapaths is to provide routes for data to travel between functional units. Datapaths can be joined together to make bigger datapaths using multiplexers [wikipedia.org].

In this lab, you are asked to design a simple Arithmetic and Logic Unit (ALU) that takes two 4-bit input data (A and B) and outputs the results (F and Cout) depending on the select signal S according to Table 1. The block diagram of the design is shown in Figure 1.




S (S1,S0)

Figure 1 Block Diagram of ALU




<strong>Table 1 ALU Functions </strong>

<table width="0">

 <tbody>

  <tr>

   <td width="30"><strong>S1 </strong></td>

   <td width="30"><strong>S0 </strong></td>

   <td width="63"><strong>F </strong></td>

   <td width="70"><strong>Cout </strong></td>

   <td width="222"><strong>Example </strong></td>

  </tr>

  <tr>

   <td width="30">0</td>

   <td width="30">0</td>

   <td width="63">A+B</td>

   <td width="70">Carry out</td>

   <td width="222">A=1100, B=1110, F=1010, Cout=1</td>

  </tr>

  <tr>

   <td width="30">0</td>

   <td width="30">1</td>

   <td width="63">A-B</td>

   <td width="70">Carry out</td>

   <td width="222">A=1100, B=1110, F=1110, Cout=0</td>

  </tr>

  <tr>

   <td width="30">1</td>

   <td width="30">0</td>

   <td width="63">A and B</td>

   <td width="70">0</td>

   <td width="222">A=1100, B=1110, F=1100, Cout=0</td>

  </tr>

  <tr>

   <td width="30">1</td>

   <td width="30">1</td>

   <td width="63">A or B</td>

   <td width="70">0</td>

   <td width="222">A=1100, B=1110, F=1110, Cout=0</td>

  </tr>

 </tbody>

</table>







<h4>3. Drawing Schematics and Simulation</h4>




Draw the circuitry for the ALU using Multisim. Make sure the inputs are labeled correctly. Simulate the circuit in Multisim.




<h4>4. Synthesis and FPGA Implementation</h4>




Synthesize and implement your design on the Basys 3 FPGA board. Use switches SW7~SW4 for input A, SW3~SW0 for input B, push button BTNU for S1 and BTND for S0, LEDs LD3~LD0 for output F, and LD4 for output Cout, as shown in following figure. Toggle input switches to observe changes on the output LEDs.

Try different inputs and verify your results.