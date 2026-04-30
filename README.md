# GENERATION-AND-DETECTION-OF-AM
# AIM:
To generate and detect the amplitude modulation and demodulation u s i n g S C I L A B and to calculate modulation index of AM.

# EQUIPMENTS REQUIRED
•	Computer with i3 Processor

•	SCI LAB
# THEORY:

Modulation can be defined as the process by which the characteristics of carrier wave are varied in accordance with the modulating wave (signal). Modulation is performed in a transmitter by a circuit called a modulator.
Need for modulation is as follows:

•	Avoid mixing of signals

•	Reduction in antenna height

•	long distance communication

•	Multiplexing

•	Improve the quality of reception

•	Ease of radiation.

Amplitude Modulation is the process of changing the amplitude of a relatively high frequency carrier signal in proportion with the instantaneous value of the modulating signal. The output waveform contains all the frequencies that make up the AM signal and is used to transport the information through the system. Therefore the shape of the modulated wave is called the AM envelope. With no modulating signal the output waveform is simply the carrier signal. Coefficient of modulation is a term used to describe the amount of amplitude change present in an AM waveform. There are three degrees of modulation available based on value of modulation index.
1)	Under modulation :	m<1, Em < Ec
2)	Critical modulation: m-1, Em = Ec
3)	Over modulation:	m>1, Em > Ec

# Algorithm
1.	Define Parameters
   
  First, define the parameters for your signals:
   
  	•	Carrier frequency (fc)
    •	Modulating signal frequency (fm)
    •	Sampling frequency (Fs)
    •	Duration of the signal (T)

2.	Create a time vector based on the sampling frequency and duration.
 
3.	Create Modulating Signal
   
    Define the modulating signal (message signal).

4.	Create Carrier Signal
   
    Define the carrier signal.

5.	Perform Amplitude Modulation
   
    Multiply the carrier signal by the modulating signal plus 1 (to ensure the modulation depth).

6. Plot the Signals
   
    Visualize the modulating, carrier, and modulated signals.

7.	Demodulate the AM Signal
   
    To demodulate, you can use envelope detection. One way is to rectify the signal and then apply a low-pass filter.

8.	Plot the Demodulated Signal
   
    Visualize the demodulated signal.

11.	Compare Signals
    
    Compare the original modulating signal with the demodulated signal.
  
# PROCEDURE

•	Refer Algorithms and write code for the experiment.

•	Open SCILAB in System

•	Type your code in New Editor

•	Save the file

•	Execute the code

•	If any Error, correct it in code and execute again

•	Verify the generated waveform using Tabulation and Model Waveform
# PROGRAM:
```
Am=10.7;
fm=1792;
fs=179200;
t=0:1/fs:2/fm;
Ac=16.05;
fc=17920;
em=Am*cos(2*3.14*fm*t);
subplot(3,1,1);
plot(t,em);
ec=Ac*cos(2*3.14*fc*t);
subplot(3,1,2);
plot(t,ec);
eam=(Ac+em).*cos(2*3.14*fc*t); 
subplot(3,1,3);
plot(t,eam);
```
# MODEL GRAPH:
<img width="919" height="1290" alt="image" src="https://github.com/user-attachments/assets/03d6ca7c-9fa1-4a92-81c6-2718308bad80" />

# OUTPUT WAVEFORM:
<img width="1609" height="974" alt="Amplitude modulation" src="https://github.com/user-attachments/assets/8a240301-27ff-415f-88da-0072aa97d35d" />


# TABULATION:
<img width="1600" height="851" alt="AM table" src="https://github.com/user-attachments/assets/e9f6e96c-3510-49c8-9180-7e8312fc6797" />
		

# Calculation:
1.	ma (Theory) = am/ac = 10.7/16.05 = 0.666
2.	ma(Practical) = (Emax-Emin)/(Emax+Emin) = 21.666/31.574 = 0.686
3.	Bw=2fmp = 2*1794.36 = 3588.72


# RESULT:
Thus the amplitude modulation and demodulation is experimentally done and the output is verified.
