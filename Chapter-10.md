# Data Representation

[toc]

## 10.01 Data Types

- Integer
  - Whole Numbers
- Boolean
  - True / False
- Date + Time
  - "10/2/2001 11:56"
- Numbers
  - Real
    - 2/10
  - Currency
    - £20
- Character
  - "A"
- String
  - "John Doe"



### Character Sets

- Computers store and process numeric and character data
- All data stored as Binary
- Character set includes Upper and Lower case letters



### ASCII

- American Standard Code for Information Interchange
- 7-Bit Code represents each character
- Codes 0-31 are control characters
- Extended ASCII Character Set



### Unicode

- Provides a unique number for every character 
- Most characters are stored as a 16-bit representation
- Unicode codes are written as : **U+0041** where **U+** represents Unicode
- Most popular Unicode Standard is UTF-8



## 10.02 Arrays

### 1D Arrays

- Python 

  - > testArray = [1 , 2, 3, 4, 5]

- Pseudo-code

  - > DECLARE MonthlySales[1:12] OF INTEGER

  - > FOR MonthlySales <-  1 TO 12
    >
    > ​                          MonthlySales[MonthlyNumber] <- 0
    >
    > ENDFOR



### 2D Arrays

- ![Java Multidimensional Array (2d and 3d Array)](https://cdn.programiz.com/sites/tutorial2program/files/java-2d-array.jpg)





## 10.03 Files

### Text Files

- > .txt



### Pseudo-Code for Text Files

- Opening a File
  - > READ
    >
    > WRITE
    >
    > APPEND

- Writing to a File

  - Filename included in `WRITEFILE` statement as program may be using more than one text file

- Reading Data From a File

  - `READ` mode used
  - File connection should be closed when no longer in use



















