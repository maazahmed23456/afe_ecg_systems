

# SAR ADC for Biomedical Applications
This project is my final year major project and is still in development. This projects aims to perfrom layout of a SAR ADC and analyse and improve upon the performance prameters. Currently the prelayout design and simulation of Sample and Hold Circuit and Comparator are completed 

*Note: Circuit requires further designing*


## A Glance at the SAR ADC 

Rapid advancements in micro-machining and microelectronics over the last few years
have accelerated the growth of implanted medical devices that greatly improve a person’s
life. These devices first gather the signals from different nodes in/on the body,
and then, they condition, multiplex, and digitize the signals. Thus, an analog-to-digital
converter (ADC), which must continuously convert a variety of analog electrophysiological
signals to digital codes, is one of the most crucial and power-hungry components.
For implantable medical devices, the successive approximation register (SAR)
ADC is a good choice. In this paper, a low-power single-ended SAR ADC architecture
is proposed to offer good compromises between power efficiency, conversion
accuracy, and design complexity. The proposed architecture supports 8-bit resolution
at a sampling rate of 1 MS/s. Using a 90-nm CMOS process with 1.8 V supply voltage

- Bootstrapped Sample and Hold Circuits
- Dynamic Latch Comparator
- Capacitive DAC
- SAR Register

## Base Paper

This project was inspired by the work of **D.M. Ellaithy**, who designed a low-power 8-bit SAR ADC for medical devices. For a detailed description of the ADC design, refer to the following paper:

Ellaithy, D.M. (2024). *A low-power 8-bit 1-MS/s single-ended SAR ADC in 130-nm CMOS for medical devices*. *Journal of Electrical Systems and Information Technology*, 11, 21. [DOI: 10.1186/s43067-024-00147-z](https://doi.org/10.1186/s43067-024-00147-z)


## Progress
Till now we have been able to do the circuit design of the bootstrapped sample and hold circuit and dynamic latch comparator and perfomr simulation in Cadence Virtuoso Suite using the gpdk090 PDK. Our next goal will be to complete the circuit design of remaining components and then perform layout.



## Block Diagram of the SAR ADC 

 <p align="center">
  <img width="800" height="500" src="/Images/block diagram.png">
</p>




## Circuit Diagram of the Sample and Hold Circuit

 <p align="center">
  <img width="800" height="500" src="/Images/BSC.jpg">
</p>

## Circuit Diagram of the Comparator Circuit

 <p align="center">
  <img width="800" height="500" src="/Images/COMPC.jpg">
</p>

## Circuit Diagram of the SAR

 <p align="center">
  <img width="800" height="500" src="/Images/SARC.jpg">
</p>

## Circuit Diagram of the DAC

 <p align="center">
  <img width="800" height="500" src="/Images/DACC.jpg">
</p>


## Pre-Layout Simulation

###  Transient Analysis of Sample and Hold


 <p align="center">
  <img width="800" height="500" src="/Images/BSS.jpg">
</p>


###  Transient Analysis of Comparator


 <p align="center">
  <img width="800" height="500" src="/Images/COMPS.jpg">
</p>



***************



## Future Work

- Design the remaining SAR logic block and Capactive DAC
- Perfrom prelayout simulation of everythihng together to show working of SAR ADC
- Perform the layout of each components and perfrom post layout simulation and verify , Complete LVS and DRC

1. **Enhance SNDR and SFDR:** Use optimized capacitor sizing and layout to minimize mismatch, enhancing signal-to-noise distortion ratio (SNDR) and spurious free dynamic range (SFDR).

2. **Improve Effective Number of Bits (ENOB):** Design a high-precision, low-offset comparator to increase accuracy, contributing to a higher ENOB.

3. **Reduce Noise:** Implement low-noise reference and power supply management techniques to suppress noise contributions from external sources.

4. **Optimize Switching Energy:** Use advanced DAC switching techniques (e.g., split-capacitor switching) to minimize power consumption and switching noise, crucial for handling low-frequency ECG signals.

5. **Fabricate and Test with Real Signals:** Plan for IC fabrication and real-time testing with ECG signal acquisition to validate performance, ensuring reliable operation in medical applications.

## Contributors 

- **Maaz Ahmed** 
- **Krishna Mouli** 
- **Sandeep** 



## Acknowledgments


- Dr.Ediga Raghuveera , AdHoc Faculty , NIT AP (mentor)
- Dr.Kiran Kumar Gurrala , Assistant Professor , NIT AP
- Dr.Puli Kishore Kumar , Assistant Professor , NIT AP
- Harika Banala , PhD , NIT AP

## Contact Information

- Shaik Maaz Ahmed , maazahmed23456@gmail.com

