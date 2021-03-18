# Chapter 03

[toc]

## 3.01 Input, Output, & Storage

### Keyboard

- Input Device
- Key moves on a plunger onto two electrical contacts
- Key has unique electric circuit
- Grid of circuits is called a key matrix
- Keyboard has its own processor
- Character Map stored in ROM



### Trackerball

- Input Device
- Ball supported by socket 
- Sensors detect movement along two axis
- Has buttons like any other mouse-like device



### Optical Mouse

- Input Device
- Uses laser tracking
- LED is reflected of surface back to CMOS
- CMOS send signal to DSP for processing



### Scanner

- Input Device
- Shines light onto Document
- Detects level of light reflected back from certain parts of document
- Light intensity converted to binary



### Inkjet Printer

- Output Device
- Print Head contains many small nozzles 
- Print Head moves horizontally via a belt and stepper motor
- **Heat**
  - Uses resistor to vaporise ink into bubbles
  - When bubble pops ink is deposited onto paper
  - Creates vacuum that attracts more ink from cartridge
- **Vibration**
  - Have Piezo crystal that receives small electrical charge
  - Forces ink out of nozzle



### Laser Printer

- Output device

- Laser beam and rotating mirror used to draw image of page on photosensitive drum

- Image converted on drum to electrostatic charge which attracts and holds toner

- Electrostaticaly charged paper rolled against drum picking up toner

- Heat used to fuse toner to paper

- Excess toner removed from drum and collected

  

### Microphone

- Input Device

- Sound vibration hits diaphragm
- Movement of diaphragm causes coil to move
- Movement of coil induces current through electromagnetic effect
- Electric current digitised
- Digital content played back through software



### 3D Printer

- Output Device

- Uses a "blueprint" file to build up layers
- 3D object created by laying down layers
- Layer is a horizontal slice of object



### Touchscreen: Resistive

- Input Device

- Construction
  - Glass Panel
  - Conductive layer
  - Metallic layer
  - Scratch resistive layer 
- When device powered up
  - Electric current runs between layers
  - When screen is touched the two layers come into contact
  - Change in electric field is noted and point is calculated by software
  - Driver software tells computer what point of screen was touched



### Touchscreen: Capacitive

- Input Device

- Construction
  - Glass Panel
  - Layer capable of storing electric charge
- When device powered up
  - User touches panel
  - Some charge transferred to user
  - Causes drop in voltage on panel
  - Software used to calculate exact coordinates of touch
  - Coordinates sent to driver software



### Speakers

- Output Device
- Different sounds caused by changes in frequency and amplitude of wave
- Take electrical signal in and translates into physical vibrations => Sound Waves
- Key Components
  - Diaphragm : connected to circular suspension at wide end and voice coil at narrow end
  - Voice Coil
  - Magnet : Placed at end of voice coil
- Usage
  - Changing polarity of current sent to electromagnet causes magnet of coil to move
  - Results in fast movements of diaphragm  causing air to vibrate thus producing sounds waves



### Hard Disk

- Storage Device
- Used for secondary storage or memory
- Has 1+ platters made from aluminium or glass mounted on central spindle
- Surface of platter is ferrous-oxide
- Disk rotated at high speed
- Each platter has read/write head positioned just above surface that can move between tracks
- Electronic circuits control movement of arms and heads 
- Surface of platter divided in concentric rings and blocks
- Data is stored in blocks and encoded as a magnetic flux pattern
- Performance limited by
  - Data transfer rate
  - Seek time
  - Latency
  - Capacity



### Optical Disk

- Storage Device
- CD / DVD
- Surface arranged in long spiral
- Plastic coated aluminium
- Data stored as pits and ridges created and read by laser beam



### Solid State Memory

- Advantages
  - No Moving parts
  - More resistant to physical shock
  - Silent
  - Lower access times
- Uses NAND Chips
- Stores data without power through use of floating gate transistors



### Sensors

- Input Device
- Used to measure some aspect of surrounding environment



### Actuators

- Output Device
- Used to interact with surrounding environment



## 3.02 Main Memory 

### RAM

- Processor is directly able to access any location by its address
- Either DRAM or SRAM Chips
- Contents lost when power removed



### DRAM

- Dynamic Random Access Memory
- Stores each bit in memory cell using sing transistor and capacitor
- Capacitor holds high or low 1 or 0
- Transistor acts as switch to allow control circuit to read or change state
- Less expensive
- Provides slower access
- Requires more power



### SRAM

- Each bit stored using state of six-transistor memory cell
- More expensive
- Provides faster access
- Requires less power

- Used for CPU Cache



### ROM

- Read  Only Memory
- Has varients
- Stores PC Boot program code [BIOS]



## 3.03 Logic Gates and Circuits

### AND

![Logic Gates - Physical design, STA & Synthesis, DFT, Automation & Flow Dev,  Verification services. Turnkey Projects](http://www.signoffsemi.com/wp-content/uploads/2020/03/and_gate-2.png)

- 2 Inputs - 1 Output



### OR

![RSD Academy - Learn for Free - Electronics Technology - Digital Circuits -  Logic Gates](https://rsdacademy.net/textbooks/DigitalCircuits/Part2/ORGate.png)

- 2+ Inputs - 1 Output



### NOT

![Make logic symbol and write Boolean expression of NOT gate.](https://haygot.s3.amazonaws.com/questions/777708_773638_ans_a65eb18b9e80492486bfe8ea55163ac3.png)

- 1 Input - 1 Output
- Returns opposite of input



### XOR

![Glossary Definition for XOR Gate](https://www.maximintegrated.com/content/dam/images/glossary/xor-gate-symbol.jpg)

- 2+ Inputs - 1 Output



### NAND

<img src="https://i.stack.imgur.com/rpqNC.png" alt="How is the NAND gate implemented? (Conceptually) - Stack Overflow" style="zoom: 50%;" />

- NOT + AND Gate



### NOR

<img src="https://projectiot123.com/wp-content/uploads/2019/05/nor-gate-truth-table.jpg" alt="Introduction to NOR Gate - projectiot123 Technology Information Website  worldwide" style="zoom:50%;" />

- OR + NOT Gate



### Constructing a Logic Circuit

- Start with Logic Expression in words
- Start with  Logic Expression in Labels



### Constructing a Truth Table

- Follow Diagram and Sketch Table based on Gates



### Efficient Circuits

- Less Gates = More Efficient

