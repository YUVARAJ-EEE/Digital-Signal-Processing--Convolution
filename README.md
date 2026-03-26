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
clc;
clear all; % clear screen
close all; % close all figure windows

% INPUT SEQUENCE
a = input('Enter the starting x(n): ');
x = input('Enter the x(n) sequence: ');
n = a:1:length(x) + a - 1;

figure(1);
stem(n, x);
xlabel('time');
ylabel('amplitude');
title('input sequence');

% IMPULSE SEQUENCE
b = input('Enter the starting h(n): ');
y = input('Enter the h(n) sequence: ');
m = b:1:length(y) + b - 1;

figure(2);
stem(m, y);
xlabel('time');
ylabel('amplitude');
title('impulse response');

% LINEAR CONVOLUTION
z = conv(x, y);
n1 = a + b : 1 : length(z) + a + b - 1;

figure(3);
stem(n1, z);
xlabel('time');
ylabel('amplitude');
title('linear convolution');
```

## OUTPUT:
![WhatsApp Image 2026-02-04 at 11 54 40 AM](https://github.com/user-attachments/assets/6aadaaca-2aba-42b6-b0eb-91fc2efb52fe)

![WhatsApp Image 2026-02-04 at 11 54 40 AM (1)](https://github.com/user-attachments/assets/0f7632c7-2069-4983-a5f6-c0b910c1073c)

![WhatsApp Image 2026-02-04 at 11 54 39 AM](https://github.com/user-attachments/assets/df3a28c0-3c3f-43d4-93ae-28cb50fa8dab)


## RESULT:
![4](https://github.com/user-attachments/assets/b8a3e47d-f384-4b13-9e47-f4e65398dab2)

