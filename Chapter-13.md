# Data Representation

[toc]

## 13.01

### User-defined Data Types

- Non-composite Data Types
  - Pointers
- Composite Data Types
  - Sets
  - Records
  - Class/Objects



## 13.02 File Organisation and Access

### Serial File Organisation

- Records are in no particular order



### Sequential File Organisation

- Records are ordered in some way



### Sequential File Access

- Serial Files
  - All data before item to be read must already have been read
- Sequential Files
  - Whole data set must have been read for item to be read



### Fixed Length Data Values



### Random Access using Record Key

- File opened in `Random` Mode
- Single record written to file using record key
- Single record can be read back using its known record key



### Direct access to Random Access File

- Retrieved via records known record key



### Direct Access to Sequentially Organised File

- Only possible if file created with fixed-length records



## 13.03 Real & Normalised Floating-Point Representation

### Format of Binary Floating-Point Real Numbers

- > 1987.381 represented as 1.987381e-3
  >
  > Fraction * 10 ^ Exponent
  >
  > number  = Fraction * 2 ^ Exponent
  >
  > Floating Point Format = Number = Mantissa * 2 ^ Exponent



### Converting Binary Floating-Point Real Numbers to Denary

- Floating point number uses 8 Bits for the Mantissa & a 4 Bit for the Exponent
- Both  a represented in Two's Complement



### Convert Denary Real Numbers into Floating-Point Representation

### Normalised Floating-Point Format

- Normalised Format is the format that preserves the maximum accuracy



### Changing Allocation of Bits in a Floating-Point Representation

### Underflow & Overflow

- Underflow occurs if number is too small to be represented by available Bits
- Overflow occurs if number is too large to be represented by available Bits



### Binary Representation may be an approximation

