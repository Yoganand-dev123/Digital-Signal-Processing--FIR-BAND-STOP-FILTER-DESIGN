# Digital-Signal-Processing--FIR-BAND-STOP-FILTER-DESIGN
## AIM:
To generate design of Band Stop FIR digital filter using Window.
## Software Required:
MAT LAB R2012.
## Algorithm:
Step 1: Open MATLAB and Write the program.

Step 2: Read the values of cut off frequency wc.

Step 2: Read the values of Order of the filter N.

Step 3: Find out the desired impulse response of the Band Stop filter Coefficient.

Step 4: Find out the windowing sequence.

Step 5: Plot the magnitude spectrum with x-label and y-label with suitable title.

Step 6: Terminate the program.

## PROGRAM: 
```
clc; % clear screen
 clear all; % clear screen
 close all; % close all figure windows
wc=input('enter the value of cut off frequency'); 
N=input('enter the value of filter'); 
alpha=(N-1)/2; 
eps=0.001; 
%Band stop
n=0:1:N-1
hd=(sin(Wc1*(n-alpha+eps))+sin(pi*(n-alpha+eps))-sin(Wc2*(n-alpha+eps)))./(pi*(n-alpha+eps))
%Hanning Window Sequence 
n=0:1:N-1; 
wh=0.5-0.5*cos((2*pi*n)/(N-1)) 
hn=hd.*wh 
% Plot the High Pass Filter with Hanning Window Technique
w=0:0.01:pi; 
h=freqz(hn,1,w);
plot(w/pi,abs(h),'blue');
```

## OUTPUT:
![dsp6(6)](https://github.com/user-attachments/assets/be998e0c-9543-48fa-bc1d-3bcc6d0cfd4e)

## RESULT:
![ds6](https://github.com/user-attachments/assets/314fae36-9ac3-469a-990b-4f60d084ecc3)

