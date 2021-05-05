# System Software

[toc]

# 16.01 Purposes of an Operating System

### Resources

- File System
- File Directory
  - Contains information for the User
  - Shows a list of files
- File Allocation Table
  - FAT
  - Block = the amount of data that can be read/written in a single operation
  - Typical allocation = 2048, 4096, 8192 bytes
  - FAT32 replaced be NTFS



### Main Memory

- Processor must have memory management strategy
- When program is complied, memory addresses are relative to the address used for first instruction in program



- Partitioned Memory
  - All memory space divided up into segments
  - Set when OS boots
  - Depending on size processes are loaded into suitable partitions
  - Dynamic partitions can be resized whenever a process completes executing

- High Level Scheduling
  - FIRST FIT
    - Load process into first partition of sufficient size
  - BEST FIT
    - Load process into partition which minimises lost space
  - WORSE FIT
    - Load process into largest available free partition



- Paged Memory Management
  - Programs divided into fixed size Pages
  - Main memory divided into segments of same size called Page Frames
  - Logical address = (1 ,112) = (PageNumber, Offset) = Byte 112 from start of Page 1
  - Not all pages need to be loaded into program for execution to start
  - Page swapping occurs as program runs to ensure that program runs smoothly
  - If too much page swapping occurs then performance degradation will happen => Thrashing



### User Interface

- Hides complexities of hardware from User
- Makes using computer much easier through the use of peripherals as compared to using commands



### Multitasking & Processes

- Modern PCs have enough Main Memory to load several programs at once
- Process = an instance of an executing program



### Processor Management

- Process States
  - Running - Process has current use of the Processor
  - Ready - Process is capable of using Processor but has to wait
  - Suspended  - Process which is not able to be run
    - Resources not sufficient
    - Waiting for signal
    - Paging system waiting for Pages to be loaded
- Strategies for low-level scheduling
  - Round Robin
  - First Ready, First Served
  - Priority Scheduling



### Interrupts & the Kernel

- Interrupt is signal to processor that some event has occurred

- OS may be capable of masking out some interrupts

- Interrupt Process by Handler

  

- Interrupts from Process
  - Save contents of all registers for LOW-PROCESS in its PCB
  - Load from PROCESS-HIGH's PCB contents of all registers
  - Mask out interrupts of a lower priority
  - Execute PROCESS-HIGH until interrupt received that PROCESS-HIGH is runnable or suspended
  - Restore PCB contents for PROCESS-LOW and restore interrupts
  - Continue execution of PROCESS-LOW

  

- Interrupts from Device



## 16.02 Virtual Machine

### Role of a VM

- System Virtual Machines
  - Emulates a complete computer system
  - Replicates functionality of  the guest OS
- Process Virtual Machines
  - Executes as a single application process under host OS
  - Used by:
    - Java Virtual Machine
    - Microsoft Virtual Machine - Common Language Runtime



### Benefits + Limitations of VMs

- Allows for the running of older software on  a newer OS
- Allows users to test a new OS before migrating





## 16.03 Translation Software

### Compiler Software

- Read Chapter 4 + PG 181
- Is the translator software required to translate high-level code into machine code
- Compiler software considers all source code statements, finds errors & produces `.exe` when all error have been fixed
- Compilation is a repetitive process 

- Key Points
  - Compiler used must match programming language + source code
  - Compiler may produce intermediate code that can be merged with compiled code from libraries
  - Once `.exe` is created neither compiler nor original code is required



### Stages in the Compilation Process

- Lexical Analysis
  - Remove Whitespace + Comments
  - Check  for errors
  - Replace all language keywords with token
  - Replace all identifier names with pointer value
- Symbol Table
  - Builds up a symbol table of identifiers & their type
  - Takes two passes through source code
- Syntax Analysis
  - Most syntactic errors are flagged by the IDE
  - Compiler flags any syntactic errors not flagged by IDE
- Code Generation + Optimisation
  - `.exe` generated



### Interpreter Software

- High-Level code can be run from any stage
- Translates each statement in program in sequence and executes them until error reached



### Pros & Cons of Compilers and Interpreters

- Compilers
  - Produces error report and `.exe`
  - Makes source code more secure
  - User unable to make changes to code
- Interpreters
  - Interpreter software must be loaded into main memory for software to execute
  - Provide better diagnostics
  - Source code less secure
  - User able to make changes



### Syntax Diagrams

<img src="https://www.teach-ict.com/as_as_computing/ocr/H447/F453/3_3_7/bnf/miniweb/images/syntax_digit1.gif" alt="Teach-ICT A Level Computing OCR exam board - program syntax diagrams" style="zoom: 67%; transform: rotate(90deg);" />

### Backus - Naur Form Notation

<img src="https://image1.slideserve.com/3265482/backus-naur-form-2-l.jpg" alt="PPT - Syntax and Backus Naur Form PowerPoint Presentation, free download -  ID:3265482" style="zoom: 33%;" />

- BNF Notation

- Is a meta language used to describe the syntax and composition of statements used to make up a high-level programming language

- > <digit> ::= 0|1|2|3|4|5|6|7|8|9|0
  >
  > <binarydigit> ::= 0|1
  >
  > <letter> ::= A|B|C|D|E|F|G|H|I|H|J|L|M|N|O|P|Q|R|S|T|U|V|W|X|Y|Z



### Reverse Polish Notation

- Infix Notation

  - > Area = Width * Length
    >
    > z = (x + y) /5

- Postfix Notation

  - > Area = Width * Length
    >
    > z = xy + 5/