# Digital-Signal-Processing--Convolution
## Aim:

                 To perform linear convolution using MAT LAB.
## Software Required:
MAT LAB R2012
## Algorithm:
Step 1: Open mat lab. Write the program.

Step 2: Read the first input sequence.

Step 3: Read the second impulse sequence.

Step 4: Plot the input sequences with x-label and y-label with suitable title. 

Step 5: Perform convolution for both the sequences using conv2() function.
  
Step 6: Plot the sequence with x-label and y-label with suitable title

Step 7: Terminate the program.

## PROGRAM:
~~~
clc; %clear screen
clear all; %clear screen 
close all; %close all figure windows 

%INPUT SEQUENCE
a=input('enter the starting x(n)');
x=input('enter the x(n) sequence');
n=a:1:length(x)+a-1;
figure(1);
stem(n,x);
xlabel('time');
ylabel('amplitude');
title('input sequence');

%IMPULSE SEQUENCE
b=input('enter the starting h(n)');
y=input('enter the h(n) sequence');
m=b:1:length(y)+b-1;
figure(2);
stem(m,y);
xlabel('time');
ylabel('amplitude');
title('impulse response');

%LINEAR CONVOLUTION
z=conv2(x,y);
n1=a+b:1:length(z)+a+b-1;
figure(3);
stem(n1,z);
xlabel('time');
ylabel('amplitude');
title('linear convolution');
~~~

## OUTPUT:
INPUT SEQUENCE

<img width="698" height="615" alt="image" src="https://github.com/user-attachments/assets/2a6d0ab6-fc40-40ea-b91e-8b0f55f72603" />

IMPLUSE RESPONSE

<img width="694" height="622" alt="image" src="https://github.com/user-attachments/assets/e6610180-099c-47c6-8717-37263d165235" />

LINEAR CONVOLUTION

<img width="695" height="616" alt="image" src="https://github.com/user-attachments/assets/edfed060-6e96-4dae-ba2c-c75cdbe35463" />

## RESULT:

![WhatsApp Image 2026-04-02 at 12 22 35](https://github.com/user-attachments/assets/96f38286-f8ba-46b9-b1b8-fc4953346690)


