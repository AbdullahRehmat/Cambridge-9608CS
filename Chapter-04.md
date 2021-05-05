## Chapter 04

[toc]

## 4.01 Von Neumann Model

- Program 
  - Sequence of instructions stored in memory
  - Data program will process
- Arithmetic Logic Unit
  - Performs Calculations on Data
- Control Unit
  - Process and executes instructions held in main memory



### Registers

- Smallest unit of storage on microprocessor
- Extremely fast 
- Classified as two types
  - General Purpose Registers
  - Special Purpose Registers
- Typical modern processor has around 8 registers
- Used to store data values read from memory or results from processing
- Registers accessible by assembly language programmer



### Accumulator

- Special Purpose Register

- Single Purpose Register



### Program Counter

- Special Purpose Register

- Program is sequence of instructions stored in consecutive memory blocks
- Program Counter hold address for memory location of next instruction



### Memory Data Register

- Special Purpose Register

- Temporarily stores data fetched from memory



### Memory Address Register

- Special Purpose Register

- Stores address about to be used by Program instruction



### Index Register

- Special Purpose Register

- Stores a number which will be used to change address value



### Current Instruction Register

- Special Purpose Register
- Stores next program instruction after it is fetched



### Status Register

- 



### ALU & System Clock

- Memory Data Register is connected directly to main memory via Data Bus
- Processor can be thought of as ALU and Control Unit working together



### Address Bus

- Carries address values
- When value is read from memory
  - Address Bus loaded with correct address
- Then Program instruction can perform operation



### Data Bus

- When read operation takes place
  - Data bus used to transport value from memory location addressed to the processor
- Bi-Directional



### Control Bus

- Made up of a number of lines each dedicated to sending or receiving a signal
- Control Signals
  - Reset
  - Memory write operation completed
  - Memory read operation completed
  - I/O operation completed
  - Interrupt received



### Performance: Bus Width

- Number of lines in address and data buses
-  8 lines means binary has range 0000 0000 1111 1111



### Performance: Clock Speed

- Each instruction has stated number of cycles it takes to complete instruction
- Number of clock cycles per instruction never change 
- Time taken for a clock cycle can change



### Performance: Ports

- Are hardware ports used to connect I/O Devices



## 4.02 Fetch Execute Cycle

| Stage                                                        | Register Transfer Notation |
| ------------------------------------------------------------ | -------------------------- |
| *Fetch Next Instruction...*                                  |                            |
| PC loaded with address of next instruction to be fetched     |                            |
| PC contents copied to MAR                                    | MAR <- [PC]                |
| PC contents are incremented for next fetch                   | PC <- [PC] + 1             |
| Address given by MAR is located and contents are copied to MDR | MDR <- [[MAR]]             |
| MDR contents are copied to CIR                               | CIR <- [MDR]               |
| *Decode the Instruction...*                                  |                            |
| Opcode and Operand are identified                            |                            |
| *Execute Instruction...*                                     |                            |
| Instruction executed                                         |                            |



### Interrupts

- Operating System Kernel is designed to recognise and interrupt
- When interrupt received
  - Processor identifies source of interrupt
  - Processor runs appropriate program (ISR) to deal with event
  - Processor returns to processing at point of interrupt



## 4.03 Processors Instruction Set

### Modes of Addressing

- Immediate Addressing 

  - Does not use an Address Value
  - LDM #13 : Load number 13 to ACC
  - LDR #27 : Load number 27 to IX

- Direct Addressing

  - Operand Value is Address to be used
  - LDD 56 : Copy contents of Address 56 to ACC
  - STO 10 : Store Contents of ACC to address 10

- Indirect Addressing

  - Operand contains address of value to be used
  - LDI 56 : Treat value found at Address 56 as Address for value to be used

- Indexed Addressing

  - Operand is added to value in IX to find address

  - LDX 50 : Address is 50 + IX Value

    

### Relative Addressing

- Calculates Address to be used from Base Address when program is loaded into Memory
- Two Base Points
  - Address of first program instruction
  - Address of current instruction
- JMP + 8 : Jump to address 8 locations from start address of program
- JMP - 9 : Jump to address 9 locations from where current instruction is loaded



## 4.04 Assembly Language

### Relationship: Assembly Language - Machine Code

| Assembly Language | Opcode    | Operand   | Machine Code        |
| ----------------- | --------- | --------- | ------------------- |
| LDM #33           | 0000 0001 | 0010 0001 | 0000 0001 0010 0001 |



### Absolute Addressing

- All address values used by program are actual address numbers
- Has implications when program is translated by assembler
- Simple Solution
  - Assembler calculates all addresses as relative addresses
  - When program runs it can occupy any memory space



### Symbolic Addressing

- Symbols used to represent addresses
- Shown in Label column in source code



### Directives

- Not a Program Instruction
- Instruction to assembler translation software to allow it to translate source code
- Can be used to include additional files
- Can be used to set aside space for variables



### Macros

- Group of instructions that can be executed multiple times in a program
- Has an identifier name that allows it to be called



### Assembler Process: 2 Pass

- Scans code twice to complete symbol table and produce final machine code
- Useage
  - Scans code first time to find any macros
  - First pass finds symbolic addresses and enters them into a symbol table
  - Second Pass occurs & complete machine code program produced









