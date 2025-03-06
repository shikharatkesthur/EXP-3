# EXP_03
# Differential Amplifier

## Introduction
The differential amplifier is a crucial analog circuit that amplifies the difference between two input signals while rejecting common-mode signals, making it essential for applications requiring precise signal amplification and noise reduction; this experiment will investigate its key parameters, including differential-mode gain, common-mode gain, and CMRR, through practical measurements and analysis of a constructed circuit, thereby providing a hands-on understanding of its operational principles.

![image](https://github.com/user-attachments/assets/34ccea41-f74b-49fa-9f6d-67fded2e402e)

## Aim
To design a differential amplifier and perform the DC Analysis, Transient Analysis and AC Analysis and extract the required parameters for the following specifications.<br>
VDD=3.2V<br>
P<=2.8mW<br>
Vicm=1.6V<br>
Vocm=1.7V<br>
Vp=0.6V<br>

## Components Used:
1. M1 and M2 (CMOSN): These NMOS transistors form the heart of the amplifier, doing the actual amplification of the difference between the input signals.

2. VDD (2V): This DC power supply provides the energy for the circuit to operate and defines the voltage range the signals can swing within.

3. R1 and R2: These load resistors convert the amplified current from the transistors into the output voltage that we measure.

4. RSS: This tail resistor sets the bias current for the transistors, which is crucial for proper operation and influences the gain.

5. V2 and V3: These are the input voltage sources, providing the signals that the amplifier will take the difference.


## Design 
Iss = P/Vdd = 2.8mW/3.2V = 0.875mA<br>
Iss = 0.875mA<br>
ID1 = ID2 = Iss/2 = 0.875m/2 =0.4375mA<br> 
ID = 0.4375mA <br>
RD = (VDD - Vocm)/ID<br> 
RD = (3.2-1.7)/0.4375m = 3.428kohm<br> 
RD = 3.428kohm<br>
Rss = Vp/Iss = 0.6/0.875mA = 685ohm<br>
Rss = 685ohm<br>

## Circuit 1 
![Screenshot 2025-03-06 225256](https://github.com/user-attachments/assets/63cf6c3f-db15-4f98-a229-b743036812e1)

## DC Analysis 
DC analysis is done to ensure whether the mosfet operates in saturation region and to 
calculate the DC operationg point of the transistor. This prevents signal distortion, which 
helps in the determination of the biasing resistors.This helps in getting a correct operating 
point despite the fluctuation in the other parameters. 

![Screenshot 2025-03-06 232248](https://github.com/user-attachments/assets/4384872a-e237-474d-856e-e404c09b15ce)

![Screenshot 2025-03-06 232445](https://github.com/user-attachments/assets/1579cd39-4432-4849-aaee-8d8b32b7985a)


Mosfet M1 and M2:<br> 

Length:180nm<br> 

Width:2.485um<br> 

## Transient Analysis:

![Screenshot 2025-03-06 232710](https://github.com/user-attachments/assets/972d4ff3-3881-4fb4-bbc7-c5bc0a8214d1)

![Screenshot 2025-03-06 232826](https://github.com/user-attachments/assets/dfd01936-f252-4321-ba8c-c2819ebff7d6)

The above two waveforms are the Vocm and Vicm. The green waveform represents the output waveform and the blue waveform represents the input waveform.

![Screenshot 2025-03-06 233212](https://github.com/user-attachments/assets/bd0f8a56-ca2e-4652-ac05-fbd61e764e42)

Voltage gain, 
     AV = Voutp-p/Vinp-p<br>
     AV=(1.87-1.54)/(1.65-1.55)<br>
     AV=3.3<br>


## AC Analysis:

![Screenshot 2025-03-06 233536](https://github.com/user-attachments/assets/3bb0c18e-2808-46ee-a440-a044eb93b214)

Gain in dB= 20log(AV)<br>
=20log(3.3)<br>
=10.37dB<br>

## Circuit 2:

Replace the resistor with a current source, Iss=0.875mV

![Screenshot 2025-03-06 234442](https://github.com/user-attachments/assets/4b7413ea-a95b-4150-b1cc-586f21b93628)

## DC Analysis:

![Screenshot 2025-03-06 234710](https://github.com/user-attachments/assets/230eb9bf-3e75-4b8a-85fa-c00f2ebc284a)


![Screenshot 2025-03-06 234809](https://github.com/user-attachments/assets/676078bb-d3ad-433d-af6d-6c12804c6697)



