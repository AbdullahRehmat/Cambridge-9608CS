# Monitoring & Control Systems

[toc]

## 18.01 Overview

### Monitoring Systems

- Monitoring System = A system designed to watch some state external to the computer system
- Event-driven System = Controller alerts the state of the system in response to some event
- Time-driven System = Controller takes action at a specific time or after a set time has elapsed
- Examples
  - Weather monitoring system
  - Pollution monitoring system
  - Car dashboard weather reading



### Control Systems

- Can be Event or Time driven
- Computer controlling circuit = direct digital control (DDC)
- Event-driven system
  - Robot loads part into work area and part is sensed as available
  - Parts moving along conveyor past an optical sensor are counted
- Time-driven system
  - Factory Buzzer sounds at set times
  - Paint heat treating stopped after set time has elapsed



### Feedback

- All the above systems use feedback.
- Sensor feedback processed by software
- Output from system fed into input alongside new data from sensors



### Hardware Requirements

- Transducers
  - Converts one form of energy to another
- Sensors
  - Devices that receive a signal and respond to it
  - Classified as
    - Thermal
    - Mechanical
    - Electrical
    - Chemical
    - Optical
- Actuators
  - A device that actuates or moves something that is connected to it
- Converts & Multiplexers
  - Physical world quantities need to be passed through a ADC to be sent to the DCC