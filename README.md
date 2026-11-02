# AMPLITUDE MODULATION

# EXP NO: 1	AMPLITUDE MODULATION using SCILAB

**AIM:**

To generate and detect the amplitude modulation using SCI LAB and to calculate modulation index of AM.

**APPARATUS REQUIRED:**

•	Computer with i3 Processor

•	SCI LAB

**THEORY:**

Modulation can be defined as the process by which the characteristics of carrier wave are varied in accordance with the modulating wave (signal). Modulation is performed in a transmitter by a circuit called a modulator.

***Need for modulation is as follows:***

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



**Note:** Keep all the switch faults in off position

**ALGORITHM:**

***1.	Define Parameters
First, define the parameters for your signals:***

•	Carrier frequency (fc)

•	Modulating signal frequency (fm)

•	Sampling frequency (Fs)

•	Duration of the signal (T)


***2.	Create a time vector based on the sampling frequency and duration.***
 
***3.	Create Modulating Signal***

Define the modulating signal (message signal).

***4.	Create Carrier Signal***

Define the carrier signal.


***5.	Perform Amplitude Modulation***

Multiply the carrier signal by the modulating signal plus 1 (to ensure the modulation depth).


***6.	Plot the Signals***

Visualize the modulating, carrier, and modulated signals.


**PROCEDURE:**

•	Refer Algorithms and write code for the experiment.

•	Open SCILAB in System

•	Type your code in New Editor

•	Save the file

•	Execute the code

•	If any Error, correct it in code and execute again

•	Verify the generated waveform using Tabulation and Model Waveform

**PROGRAM:**
~~~

fm=295;
Am=2.48;
fc=10*fm;
Ac=1.8*Am;
fs=10*fc;
t=0:1/fs:2/fm;
em=Am*sin(2*3.14*fm*t);
ec=Ac*sin(2*3.14*fc*t);
eAM=(Ac+em).*sin(2*3.14*fc*t);
subplot(3,1,1);
plot(t,em);
subplot(3,1,2);
plot(t,ec);
subplot(3,1,3);
plot(t,eAM);

~~~


**OUTPUT WAVEFORM:**

<img width="1123" height="613" alt="Exp 1 output" src="https://github.com/user-attachments/assets/4215296b-c89c-45bb-94ab-686272ed1733" />




**TABULATION:**

<img width="3165" height="2014" alt="IMG_20261102_191804_edit_140339349058793 jpg" src="https://github.com/user-attachments/assets/fd0e1946-4976-4df9-8763-cb05493fed25" />




**CALCULATION:**

<img width="2314" height="3193" alt="IMG_20261102_211246_edit_141876510743975 jpg" src="https://github.com/user-attachments/assets/6f05ee73-6507-4508-97e5-b65b17ba863c" />



**MODEL GRAPH:**

 <img width="919" height="1290" alt="image" src="https://github.com/user-attachments/assets/55326c5b-7dd5-4873-aaf6-d219bb7c4420" />

 
 


**RESULT:**

Thus the amplitude modulation is experimentally done and the output is verified.
