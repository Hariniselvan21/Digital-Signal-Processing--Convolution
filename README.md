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

```
clc; % clear screen

clear all; % clear screen

close all; % close all figure windows

% INPUT SEQUENCE

a=input('enter the starting x(n)');

x=input('enter the x(n) sequence');

n=a:1:length(x)+a-1;

figure(1);

stem(n,x);

xlabel('time');

ylabel('amplitude');

title('input sequence');

% IMPULSE SEQUENCE

b=input('enter the starting h(n)');

y=input('enter the h(n) sequence');

m=b:1:length(y)+b-1;

figure(2);

stem(m,y);

xlabel('time');

ylabel('amplitude');

title('impulse response')

% LINEAR CONVOLUTION

z=conv2(x,y);

n1=a+b:1:length (z)+a+b-1;

figure(3);

stem(n1,z);

xlabel('time');

ylabel('amplitude');

title('linear convolution');
```
## OUTPUT:
![WhatsApp Image 2025-10-13 at 19 27 02_fe1f378b](https://github.com/user-attachments/assets/731194a2-5acb-4300-8d2a-d522cd4c4262)


## RESULT:

![WhatsApp Image 2025-11-24 at 20 00 04_5d056374](https://github.com/user-attachments/assets/cc53a629-c887-4c62-990d-2ec353822635)
