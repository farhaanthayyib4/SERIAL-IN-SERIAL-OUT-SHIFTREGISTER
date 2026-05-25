# SERIAL-IN-SERIAL-OUT-SHIFTREGISTER

**AIM:**

To implement  SISO Shift Register using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

**SISO shift Register**

A Serial-In Serial-Out shift register is a sequential logic circuit that allows data to be shifted in and out one bit at a time in a serial manner. It consists of a cascade of flip-flops connected in series, forming a chain. The input data is applied to the first flip-flop in the chain, and as the clock pulses, the data propagates through the flip-flops, ultimately appearing at the output.

The logic circuit provided below demonstrates a serial-in serial-out (SISO) shift register. It comprises four D flip-flops that are interconnected in a sequential manner. These flip-flops operate synchronously with one another, as they all receive the same clock signal.

![image](https://github.com/naavaneetha/SERIAL-IN-SERIAL-OUT-SHIFTREGISTER/assets/154305477/e81c4072-37f9-46c6-8145-566764b74c3a)

Figure 01 4 Bit SISO Register

The synchronous nature of the flip-flops ensures that the shifting of data occurs in a coordinated manner. When the clock signal rises, the input data is sampled and stored in the first flip-flop. On subsequent clock pulses, the stored data propagates through the flip-flops, moving from one flip-flop to the next.
Each D flip-flop in the circuit has a Data (D) input, a Clock (CLK) input, and an output (Q). The D input represents the data to be loaded into the flip-flop, while the CLK input is connected to the common clock signal. The output (Q) of each flip-flop is connected to the D input of the next flip-flop, forming a cascade.

**Procedure**

/* write all the steps invloved */

**PROGRAM**
```
/* Program for flipflops and verify its truth table in quartus using Verilog programming.
Developed by: UDHAYDHARSHAN S
RegisterNumber: 212225230286
*/
module deexp2(a,b,c,d,f1,w,x,y,z,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1=((~b&~d)| (~a&b&d)| (a&b&~c));
assign f2=((~y&z)|(x&y)|(w&y));
endmodule

```
RTL realization

<img width="907" height="592" alt="image" src="https://github.com/user-attachments/assets/25c80ef5-5bc3-458d-a083-fe1a57232257" />

**RTL LOGIC FOR SISO Shift Register**

<img width="937" height="332" alt="image" src="https://github.com/user-attachments/assets/cf676b81-c69b-4309-a2b1-7dc9fd1ad11e" />


**TIMING DIGRAMS FOR SISO Shift Register**

<img width="946" height="398" alt="image" src="https://github.com/user-attachments/assets/1743fa03-d9cb-47e8-ab16-23d6c47f0b33" />

**RESULTS**
Thus the given logic functions are implemented using and their operations are verified using Verilog programming.
