# Tomasulo-Algorithm-Simulation
This Repository features a simulation of the tomasulo's algorithm used in dynamic scheduling using javascript and react frontend

There are currently only 6 instructions implemented:
L.D (load)
S.D (store)
ADD.D (add float)
SUB.D (sub float)
MUL.D (mult float)
DIV.D (div float)

the format for the instructions is given in the following example (MIPS 64 assembly):
L.D F0, 20
SUB.D F4, F0, F2
ADD.D F4, F4, F2
MUL.D F4, F4, F2
DIV.D F4, F4, F4
S.D F4, 20


note that in L.D and S.D effective address is immediately written instead of base register + offset (instead of L.D F0, 0(R1) we write L.D F0, 20) where 20 is the effective address resulting from 0 + value stored in register R1
---------------------------------------

****************************************************
INSTRUCTIONS ON HOW TO USE ALGORITHM:

1. Input the assembly code following the given above format
2. write the latency of the instructions (time each instruction takes in buffer)
3. click LOAD INSTRUCTIONS button to load instructions into the instruction queue
4. click EXECUTE CYCLE to execute the cycle and move to the next cycle till all instructions are executed and written to the memory at the end
note that memory address size is 21 and reigster file goes from F0 till F9
****************************************************
