<img width="1920" height="1080" alt="V at 1k, 10k" src="https://github.com/user-attachments/assets/4817a3d0-2130-4b20-87f3-e44245b89c0a" /><img width="1920" height="1080" alt="V at 1k,1k" src="https://github.com/user-attachments/assets/67250db1-8170-4492-8dd1-01493a07b05e" /># Voltage Divider Behavior Analysis

## Overview
This project focuses on simulating a basic voltage divider in LTSpice and studying how the output voltage changes when resistor values are varied. Voltage dividers are one of the most fundamental concepts in electronics and are widely used for biasing, reference generation, and signal scaling.

## Circuit Setup
The circuit consists of:
- A 1V DC voltage source  
- Two resistors (R1 and R2) connected in series  
- Ground connection  
- Output node taken from the junction between R1 and R2  

The voltage at this junction is what we analyze as the output.

## Observations
1. **R1 = 1kΩ, R2 = 1kΩ**  
   - The output voltage was around 0.5V.  
   - As expected, the symmetrical resistor values divided the input voltage equally.  

   <img width="1920" height="1080" alt="V at 1k,1k" src="https://github.com/user-attachments/assets/172a3af1-2260-4cd6-8ff1-b4f904afef4a" />

2. **R1 = 10kΩ, R2 = 1kΩ**  
   - The output voltage dropped to about 0.09V.  
   - Since R1 is much larger than R2, most of the input voltage is dropped across R1.  

   <img width="1920" height="1080" alt="V at 10k, 1k" src="https://github.com/user-attachments/assets/c828aa5f-cda4-47c4-bf4e-bf82d4bdac8c" />

3. **R1 = 1kΩ, R2 = 10kΩ**  
   - The output voltage increased to about 0.91V.  
   - With R2 much larger than R1, most of the voltage appears across R2, pushing the output closer to the input voltage.  

   <img width="1920" height="1080" alt="V at 1k, 10k" src="https://github.com/user-attachments/assets/67161937-250d-4636-9aa9-6d9ea6a72b50" />

## Conclusion
The output of a voltage divider is determined by the ratio of R1 and R2. By adjusting resistor values, the voltage at the output can be tuned anywhere between the supply and ground. This simple concept is essential for many analog applications like biasing amplifiers or reducing voltage levels for measurement.

## Files and Images
- The LTSpice simulation files are included in the `Circuit Files` folder.  
- Output waveform images are placed in the `Images` folder.  
