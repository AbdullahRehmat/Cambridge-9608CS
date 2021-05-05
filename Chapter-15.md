# Hardware

[toc]

## 15.01 Logic Gates and Circuit Design

### Truth Tables

<img src="https://instrumentationtools.com/wp-content/uploads/2018/10/Logic-Gates-and-Truth-tables.png" alt="Logic Gates and Truth tables - Inst Tools" style="zoom: 80%;" />



### The Half Adder

<img src="https://projects-static.raspberrypi.org/projects/halfadder/fbd927fdbca5dcb6631fad44fa49ec03feafd80c/en/images/fig1.png" alt="Building a Half Adder - Introduction | Raspberry Pi Projects" style="zoom:30%;" />

- Two inputs are each a binary digit to be added together
- Two outputs show value of the addition and carry bit



### The Full Adder

- Circuit for Half-Adder with the addition  of a carry bit for the two bit addition
- Therefore the circuit has
  - 3 Inputs: A, B, C
  - 2 Outputs: Sum + Carry



## 15.02 Boolean Algebra

### Notation

| Boolean Operator | Algebraic Notation | Example | Meaning |
| ---------------- | ------------------ | ------- | ------- |
| OR               | +                  | X + Y   | X OR Y  |
| AND              | .                  | X . Y   | X AND Y |
| NOT              | x̅                  | x̅       | NOT X   |



### Simplification of Boolean Expressions

| Given Expression  | Simplification                          |
| ----------------- | --------------------------------------- |
| 2X + 6Y           | 2 (X + 3Y)                              |
| PQ + PQR          | PQ (1 + R)                              |
| AC + BC + AD + BD | C (A + B) + D (A + B) = (C + D) (A + B) |



### Boolean Identities

- A. A + A
- A + A + A
- A +  ā  = 0
- A +  ā  = 1
- A. I = A
- A + I = I
- A. 0 = 0
- A + 0 = A



| Identity Name    | Expression                            | Comment                                                      |
| ---------------- | ------------------------------------- | ------------------------------------------------------------ |
| Commutative Law  | A + B = A + B           A . B = A . B | Order can be changed, for a logic circuit inputs can be reversed |
| Associative Law  | A + (B + C) = (A + B) + C             | Brackets could have been omitted                             |
| Distributive Law | A. (B + C) = (A + C) . (A + C)        | This is like the expansion of brackets in algebra            |



### De Morgan's Law

- A NAND Gate behaves as two inputs to an AND Gate, followed by the output into a NOT Gate
- A NOR Gate behaves as two inputs to an OR Gate, followed by the output into a NOT Gate



## 15.03 Karnaugh Maps

- Used to simplify Boolean Expression



## 15.04 Flip Flops

### The SR Flip Flop

<img src="https://circuits-diy.com/wp-content/uploads/2020/02/SR-Flip-Flop-Circuit-74HC00-Truth-Table-1280x720.png" alt="SR Flip Flop Circuit 74HC00 - Truth Table" style="zoom:50%;" />

- A one-bit memory device with two inputs

- S input (SET) causes the output to be set to 1

- R input (RESET) causes the output to be set to 0

- If the low state is significant then the inputs are labelled bar R and bar S

- Storage

  - Several Flip Flops can be used to store a byte

  

### The JK Flip Flop

<img src="https://circuits-diy.com/wp-content/uploads/2020/02/JK-Flip-Flop-Circuit-using-74LS73-Truth-Table.png" alt="JK Flip Flop Circuit using 74LS73 - Truth Table" style="zoom:50%;" />

- Most widely used Flip Flop Design



## 15.05 RISC Processors

### Background

- Developed in early 1990's
- Development has been slowed by the lack of software written to run on RISC
- Intel X86 Families' Dominance
- Devices using RISC Include
  - Playstation 3 
  - XBox 360
  - Televisions
  - Smartphones



### CISC vs RISC

| CISC                                             | RISC                                        |
| ------------------------------------------------ | ------------------------------------------- |
| Limited number of general purpose registers      | Large number of general purpose registers   |
| Number of clock cycles taken by instruction vary | Each instruction takes a single clock cycle |
| Instructions are a variable length               | All instructions are a fixed byte size      |
| Hundreds of instructions                         | Reduced number of instruction               |
| Exclusive use of cache memory                    | Instructions + Data are held in RAM         |



### Pipelining

- CISC: Fetch Decode Execute cycle
- RISC: Fetch, Decode, Execute, Access operand in memory, Write result to register



### Problems with Pipelining

- Data dependency
- Branch Instructions



### Interrupt Handling

- Signal is sent to processor from hardware device to indicate that the device needs attention



## 15.06 Parallel Processing

### Single Instruction, Single Data (SISD)

- Computer system has a single processor with one data source which works on a single algorithm
- Overall task is coded as a sequence of tasks
- Sequential Processing



### Single Instruction, Multiple Data (SIMD)

- Array of vector processing



### Multiple Instruction, Single Data (MISD)

- Many processors perform operations on same data value
- Data may be value from array
- Nodes merge data values into final result



### Multiple Instruction, Multiple Data (MIMD)

- Has a number of processors that function independently and simultaneously for different data values

















