### ENCODER 8TO3 DATAFLOW Modelling

**AIM:**

To implement  Encoder 8 To 3 in Dataflow Modelling using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:** Quartus prime

**THEORY**

**Encoder 8 To 3**

The 8 to 3 line Encoder is also known as Octal to Binary Encoder. In 8 to 3 line encoder, there is a total of eight inputs, i.e., D0, D1, D2, D3, D4, D5, D6, and D7 and three outputs, i.e., A0, A1, and A2. In 8-input lines, one input-line is set to true at a time to get the respective binary code in the output side. Below are the block diagram and the truth table of the 8 to 3 line encoder.

<img width="1490" height="628" alt="image" src="https://github.com/user-attachments/assets/226afa7d-ca57-42e8-9ddc-172229edbff3" />


Figure 01  Block Diagram of Encoder 8 * 3

**Truth Table**

<img width="425" height="322" alt="image" src="https://github.com/user-attachments/assets/7e203034-8291-48c3-a80e-52a1231c79fe" />


The logical expression of the term A0, A1, and A2 are as follows:

A0 = D1 + D3 + D5 + D7

A1 = D2 + D3 + D6 + D7

A2 = D4 + D5 + D6 + D7

Logical circuit of the above expressions is given below:

<img width="791" height="496" alt="image" src="https://github.com/user-attachments/assets/aedc3a8c-9d43-431b-b39c-5fdeb6b3e1c8" />


Figure 02  Encoder 8 * 3

**Procedure**
Type the program in Quartus software.

Compile and run the program.

Generate the RTL schematic and save the logic diagram.

Create nodes for inputs and outputs to generate the timing diagram.

For different input combinations generate the timing diagram.


**PROGRAM**

module exp5(din,a,b,c);

input [0:7] din;

output a,b,c;

assign a=(din[4]| din[5]| din[6]| din[7]);

assign b=(din[2]| din[3]| din[6]| din[7]);

assign c=(din[1]| din[3]| din[5]| din[7]);

endmodule


Developed by: RegisterNumber:*/
Sundaresh/25006077

**RTL LOGIC FOR Encoder 8 To 3 in Dataflow Modelling**
<img width="1334" height="908" alt="image" src="https://github.com/user-attachments/assets/e84f36b5-c9ef-441c-8cb2-613387ab9a24" />

**TIMING DIGRAMS FOR Encoder 8 To 3 in Dataflow Modelling**
<img width="1921" height="1201" alt="image" src="https://github.com/user-attachments/assets/6b8b0172-4026-4286-9180-f0a2b1603116" />

**RESULTS**
Thus Encoder 8 To 3 in Dataflow Modelling using verilog and validating their functionality using their functional tables is implemented and verified.



