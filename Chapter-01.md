# Chapter 01

[toc]

## **1.01: Number Representation** 



### Denary System

- 0 1 2 3 4 5 6 7 8 9
- Base-10



###  Binary System

- Only 0 & 1

![img](https://lh4.googleusercontent.com/mkJvVGjIGW2DKEwN3pzAI-c9N4BD0fZm9KiEtl1YLQSSk0Kgs8W_xln_C0biigwIzvKQoX2CujFers2z1ujm-wJXUbqt36dvURF6moCendKMpxYvLNMad4leG5PTzXeIy7-BtvWg)



### Hexadecimal System

- 0 1 3 4 5 6 7 8 9 A B C D E F

- Base-16

  

###  Conversion Between Systems

- Convert Binary to Hex

- - Split into 4-Bit Bytes
  
  - Convert each byte to Denary
  
  - Represent Denary as Hex
  
    

### Numbers in a Computer

- All data stored as Binary
- Most significant bit has place value of 128
- Least significant bit has place value of 0 or 1



### Two’s Complement Representation

- Allows for both positive and negative integers
- Sign & Magnitude not included in course
- Two’s Complement place values 



| -128 | 64   | 32   | 16   | 8    | 4    | 2    | U    |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- |
|      |      |      |      |      |      |      |      |



### Representing Characters

- All data must be represented in main memory
- ASCII or Unicode will be used



### Binary Coded Decimals

- Binary representation that can be used for a positive denary integer
- Each digit is represented in sequence with a group of four binary digits

| 8                    |      | 5    |      | 9    |
| -------------------- | ---- | ---- | ---- | ---- |
| 1000                 |      | 0101 |      | 1001 |
| => 859 = 10001011001 |      |      |      |      |



## **1.02: Images**



### Bitmapped Image

- Rectangular graphic made up of pixels
- The color of each pixel is represented as a binary pattern
- Monochrome = black & white
- 16 Color = 16 possible colors
- 256 Color = 256 possible colors
- 24-Bit Color = True color, millions of colors available

| Bitmap Encoding | Pixel Representation | Explanation          |
| --------------- | -------------------- | -------------------- |
| Monochrome      | 1 Bit                | Byte stores 8 Pixels |
| 16 Colors       | 4 Bits               | Byte stores 2 Pixels |
| 256 Colors      | 8 Bits               | Byte stores 1 Pixel  |
| 24-Bit Color    | 24 Bits - 3 Bytes    | 224 Colors           |

- Bitmap file header will store data
- Header data contains height and width of image and encoding
- Drawbacks include, if image overstretched pixels will become visible
- Better viewed on small screen with high PPI count



### Vector Graphics

- Graphic made up from a number of “objects”
- Objects are organised into “shape libraries” and have properties
- Properties determine size and appearance of object
- If object is resized then size is recalculated therefore easily scalable



## **1.03: Sound**

### Sound

- Sound is an analogue signal

- Convert to analogue from digital via an ADC

- Sound sampled at set intervals

- Samples form binary values which form sound file

- Issues affecting sound quality include:

- - Sample Resolution: How many bits are used to encode each sample value
  - Sample Rate: How often are samples taken. How many values per second

- Editing Software:

- - Sound input via microphone
  - Can digitise an analogue sound source
  - Cutting and pasting sections of audio
  - Filtering out certain sounds
  - Normalising recording level
  - Exporting audio into various formats



## **1.04: Video**

### Video

- Frame-rate is the frequency at which frames are played

Progressive Encoding:

- System stores data for the entire frame and displays all frame data at the same time.
- Frame rate = Number of pictures per second.

Interlaced Encoding:

- Some devices cannot display all frame data at same time like TVs

- Data from single frame is encoded in two fields

- - Field 01: All even rows
  - Field 02: All odd rows

- Image is rendered by switching between even and odd fields

- Rate of picture display is 2x frame rate

- Picture frames that make up interlaced fields have a relative order to each other

- - Spatial order shows which should be odd or even
  - Temporal order refers to field or frame which represents earlier moment
  - If either of the above is incorrect playback will be jerky



## **1.05: Compression Techniques**

### Image Compression Techniques

### Run Length Encoding

- A form of lossless data compression in which runs of data (sequences in which the same data value occurs in many consecutive data elements) are stored as a single data value and count, rather than as the original run. This is most useful on data that contains many such runs.

### Lossless encoding

-  Lossy compression or irreversible compression is the class of data encoding methods that uses inexact approximations and partial data discarding to represent the content.

Video Compression Techniques

### Spatial Redundancy

- Run Length Encoding for videos

### Temporal Redundancy

-  Filters. Pixels in two video frames that have the same values in the same location.

### File Formats

- Images
  - .PNG
  - .JPG
  - .GIF
  - .BMP
- Video
  - AVI ( standard Microsoft Windows container)
  - MOV ( standard QuickTime container)
  - .MP4
  - Matroska ( Open Source )
- Sound
  - .MP3
- Formats are chosen based on their **popularity**, **overheads**, and **support** available.

## Summary

- Numbers can be written as Binary, Denary, or Hexadecimal
- Two's complement allows for both positive and negative numbers to be represented
- Binary-Coded decimals ( BCD ) is a coding system for positive integers
- Images can be made up of pixels - bitmap
- Vectors are constructed by drawing objects from libraries
- Sound is encoded samples taken from an analogue source at a set sampling rate
  - Sampling resolution defines quality
- Videos are a sequence of images played at high speed  accompanied by a soundtrack
- Compression is either 'lossy' or 'lossless'