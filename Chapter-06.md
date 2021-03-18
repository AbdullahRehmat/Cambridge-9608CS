# Chapter 06

[toc]

## 6.01 Data Security

### Security: Computer System

- User Accounts
  - Have a Password
- Firewalls
  - Can be implemented in hardware or software
  - Used to prevent unauthorised network access
  - Examines all messages entering and leaving a network
  - Techniques
    - Packet Filtering: Packets accepted or rejected based on set rules
    - Application Gateway: Security checking applied to Telnet, FTP, etc.
    - Proxy Server: Hides true network addresses
  - Static Packet Filtering examines packet based on information stored in header + fixed rules
  - Dynamic Packet Filtering
    - Examines header data
    - Examines packet contents
    - Monitors state of connection and compiles information in  a state tables
- Authentication Techniques
  - Passwords
  - Biometrics
  - Digital Signatures



### Security: Data

- Disk Mirroring
  - Have two identical copies of data on different servers
  - Having frequent automated backups
- Encryption
  - Is a safeguard to protect security of data
  - Original file has all data bytes changed in by encryption key
  - File is meaningless until decryption key is provided
- Authorisation
  - Individual files can be password protected
  - Users and User Groups can be created to define permissions
- Logs
  - If an error occurs system should log event per user



## 6.02 Data Integrity

### Data Validation

- Check Digit

  - Extra character is added to important field to make sure that it is transmitted as entered

- Selected Values from List

  - Certain data values are only possible and are taken from a list of permitted values

- Range Check

  - Checks if value is between a certain range

- Format Check

  - Product code must follow a certain format

- Length Check

  - Value must be certain length

- Presence Check

  - Field must contain value

- Uniqueness Check

  - Data Value cannot be repeated

- Data Verification for Data Entry

  - Data Verification

    - May take place on one or more value entered
    - Checks if two values are the same

  - Data Verification during Transfer

    - Verification checks if data copied is same as the source

  - Parity Check

    - Checks validity of the codes of individual characters within a file when it is read from or written to

  - Parity Block Check

    - Parity check can be made of a group of bytes when transmitted in a sequence
    - Data for parity bite is calculated and added to the block sequence

    



















































