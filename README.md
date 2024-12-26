### SYNCHRONOUS-UP-COUNTER

**AIM:**

To implement 4 bit synchronous up counter and validate functionality.

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

**4 bit synchronous UP Counter**

If we enable each J-K flip-flop to toggle based on whether or not all preceding flip-flop outputs (Q) are “high,” we can obtain the same counting sequence as the asynchronous circuit without the ripple effect, since each flip-flop in this circuit will be clocked at exactly the same time:

![image](https://github.com/naavaneetha/SYNCHRONOUS-UP-COUNTER/assets/154305477/d5db3fa0-e413-404c-b80e-b2f39d82e7e8)


![image](https://github.com/naavaneetha/SYNCHRONOUS-UP-COUNTER/assets/154305477/52cb61eb-d04b-442d-810c-31185a68410b)

Each flip-flop in this circuit will be clocked at exactly the same time.
The result is a four-bit synchronous “up” counter. Each of the higher-order flip-flops are made ready to toggle (both J and K inputs “high”) if the Q outputs of all previous flip-flops are “high.”
Otherwise, the J and K inputs for that flip-flop will both be “low,” placing it into the “latch” mode where it will maintain its present output state at the next clock pulse.
Since the first (LSB) flip-flop needs to toggle at every clock pulse, its J and K inputs are connected to Vcc or Vdd, where they will be “high” all the time.
The next flip-flop need only “recognize” that the first flip-flop’s Q output is high to be made ready to toggle, so no AND gate is needed.
However, the remaining flip-flops should be made ready to toggle only when all lower-order output bits are “high,” thus the need for AND gates.

**Procedure**

Type the program in Quartus software.

Compile and run the program.

Generate the RTL schematic and save the logic diagram.

Create nodes for inputs and outputs to generate the timing diagram.

For different input combinations generate the timing diagram.

**PROGRAM**

/* Program for flipflops and verify its truth table in quartus using Verilog programming. 

Developed by:saranya.j RegisterNumber:24900574
*/


![Screenshot 2024-12-26 190959](https://github.com/user-attachments/assets/19ef7d93-3c4a-47b0-9c13-83becbd0f1b1)



**RTL LOGIC UP COUNTER**

![Screenshot 2024-12-26 191016](https://github.com/user-attachments/assets/6a063cf5-b071-45e1-ab6e-90c302c9448e)


**TIMING DIAGRAM FOR IP COUNTER**

![Screenshot 2024-12-26 191032](https://github.com/user-attachments/assets/1da111ea-48d9-4a1a-95a5-a99cad093f63)



**TRUTH TABLE**

![Screenshot 2024-12-26 191041](https://github.com/user-attachments/assets/ec44e5b4-290e-4ada-bb00-511c07d89cea)



**RESULTS**

Implement 4 bit synchronous up counter and validate functionality is verified.

