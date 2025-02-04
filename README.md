
# Lab 1: Knowing Your Instruments 
Aashika Uppala, Megan Fister

2/3/2025

## Introduction
The goal of this lab is to familiarize students with essential electronic test equipment, including a digital multimeter, an oscilloscope, a function generator, and direct power supply. 
Understanding these instruments is critical for future experiments. 
Introduction of Summary: The purpose of this lab is to introduce students to key electronic test instruments. Gaining proficiency with these tools is essential for conducting future experiments effectively.
We performed various measurements using the provided equipment to verify component values and signal characteristics. Tasks include measuring resistances, capacitances, and voltage outputs, as well as analyzing waveforms using an oscilloscope.
Finally, we learned to use GitHub for collaboration and documentation.
By completing this lab, students gained hands-on experience in using electronic test instruments, verifying expected values against measured data, and analyzing discrepancies.
The exercise also introduced GitHub as a documentation and collaboration tool.

## Methods
### Lab Equipment
• A Digital Multimeter

• A Function Generator

• An Oscilloscope

• A computer with access to the internet

• Four different resistors (any value)

• Four different capacitors (any value, at least one electrolytic)

• A DC Power supply

• A 10KΩ resistor

#### Objective 1: Use the above-listed lab equipment to measure and verify equipment, component, and circuit values.

Important note: make sure everything is being measured in DC!

*Using the Fluke Digital Multimeter (DMM)*

*Step 1: Measure and verify the resistance of various resistors.*

PLug a black wire into the "COM" port and a red wire into the port labeled V&omega;. Wrap each end of a resistor around the metal ends of each wire, turn the knob to mesure ohms, and record the resistance measured. Compare the measured value to the expexcted value based on the color code of the resistor. Repeat for all four resistors.

![Resistors](https://github.com/aashikauppala/BAE-305-Labs/blob/main/Lab1%203.jpg)

*Step 2: Measure and verify the capacitance of various capacitors.*

Keep wires plugged in and connect the alligator clips to the metal end of the wires. Connect these clips to either end of the capacitor and record the capacitance measured. Compare the measured value to the expexcted value based on the code of the capacitor.

![Capacitors](https://github.com/aashikauppala/BAE-305-Labs/blob/main/Lab1%203.jpg)

*Using the D.C. Power Supply (DCPS)*

*Step 3: Measure and verify the voltage output of the DCPS.*

Plug in and turn on the DCPS and then connect the red and black wires to the ports labeled "main output" and "1-20 VDC." Set the main output current to the minimum and the voltage to 1.5V. Clip the alligator clamps from the wires connected to the Fluke DMM to the wires plugged into the DCPS. Turn the knob on the Fluke DMM to measure voltage. Repeat this for 7.0V and then 12.0V. Then, reconnect the red and black wires to the "Aux 2" and "12 VDC" ports and measure voltage and then repeat with the "Aux 1" and "3.5/5 VDC" ports.

*Using the Function Generator (FG) and Oscilloscope*

*Step 4: Measure and verify the function generator output.*

Connect a 10K&omega; resistor to the output of the FG and set the FG to produce a 2kHz sine wave of maximum amplitude. Measure the amplitude and frequency of the wave using four strategies: counting the squares on the screen of the oscilloscope, moving the cursors on the oscilloscope, using the measurement features on the oscilloscope, and connecting the wires of the Fluke DMM. 


## Results
*Step 1: Measure and verify the resistance of various resistors.*

| Color Code | Expected Resistance &Omega; | Tolerance | Maximum | Minimum | Measured | Range |
|:---|:---:|:---:|:---:|:---:|:---:|---:|
| Brown-Black-Black-Gold | 10    | 5%|10.5   | 9.5   | 10.1  | In Range |
| Brown-Green-Brown-Gold | 150   | 5%|157.5  | 142.5 | 147.7 | In Range |
| Orange-Orange-Red-Gold | 3310  | 5%|3465   | 3135  | 3310  | In Range |
| Brown-Green-Green-Gold |1500000| 20%|1575000|1425000|1495000| In Range |

*Step 2: Measure and verify the capacitance of various capacitors.*

Assume 20% tolerance for capacitor 4 where there is no tolerance labeled. 

| Color| Type | Expected Capacitance (pF) | Maximum (pF) | Minimum (pF) | Measured (pF) | Range |
|:---|:---:|:---:|:---:|:---:|:---:|---:|
|   yellow   | ceramic      |1000     | 1100  | 900  | 1320        | Out of Range |
| yellow   | ceramic      |22      | 23.1     | 20.9     | 320       | Out of Range |
| yellow    | ceramic | 1000000  | 1800000   | 800000  | 1160000   | In Range |
| black     | electrolytic | 100000000  | 120000000 | 80000000   | 97200000    | In Range |


*Step 3: Measure and verify the voltage output of the DCPS.*

- While the DCPS is set at 1.5 V, the DMM is bouncing from 1.477 V to 1.525 V.
- While the DCPS is set at 7 V, the DMM measures 7 V.
- While the DCPS is set at 12 V, the DMM measures 12 V.
- When connected to the 3.5/5 VDC port in the DCPS, the DMM measures 5.230 V (no matter the voltage on power supply).
- When connected to the 12 VDC port in the DCPS, the DMM measures 12 V (no matter the voltage on power supply).


*Step 4: Measure and verify the function generator output.*

1. "Counting squares" on the oscilloscope screen
2. Using the moveable cursor on the oscilloscope
3. Using the measurement features of the oscilloscope
4. Fluke DMM


|  |  Frequency (Hz)|  Voltage (V)|
|:---|:---:|:---:|
|1   |2000 |6|
|2     | 1869 |6.16|
|3     | 1905 |6.16|
|4     | 1854 |4.149|


## Discussion
*Resistors*

*Do the resistors fall within their tolerance?*

Some measured values differed slightly from expected values due to instrument tolerances. However, all of the resistors fall within their range of tolerance. 


*Capacitors*

*Do the instruments agree with the expected value? Does polarity affect the measurement of the electrolytic capacitor?*

The instruments agree with the expected value for the most part. Two of the capacitors were out of range. Capacitor 2 is too small to measure with these instruments and capacitor 1 was higher than the expected value. Polarity affects the measurement of the electrolytic capacitor, but not enough to cause it to be outside of the expected range. 


*DCPS*

*Do the instruments agree with each other? Why?*

The oscilloscope provided more precise waveform measurements than the DMM. The power supply's meter readings were close but not always exact compared to the DMM.


*Function Generator and Oscilloscope*

*Do the instruments agree? Why?*
Frequency and amplitude varied slightly across different measurement techniques, but they agree for the most part. The oscilloscope’s measurement feature provided the most accurate reading. Differences between instruments highlight the importance of calibration and understanding tool limitations. Probe resistance must be accounted for when measuring low-resistance values.

## Conclusion
This lab provided essential hands-on experience with electronic measurement instruments. We learned to verify component values, analyze signals, and compare measurements from different tools.
The experience with GitHub will facilitate effective collaboration and documentation for future labs. Understanding instrument limitations and proper measurement techniques is crucial for accurate electronic analysis.
