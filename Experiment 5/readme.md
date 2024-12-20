# Aim:
1. To perform Linear Convolution using Circular Convolution. 
2. To perform Circular Convolution using Linear Convolution.
# Theory:
Performing Linear Convolution Using Circular Convolution 
Method: 
1. Zero-Padding: 
o Pad both sequences x[n] and h[n] with zeros to a length of at least 2N-1, 
where N is the maximum length of the two sequences. This ensures that the 
circular convolution will not wrap around and introduce artificial 
periodicity. 
2. Circular Convolution: 
o Perform circular convolution on the zero-padded sequences. 
3. Truncation: 
o Truncate the result of the circular convolution to the length N1 + N2 - 1, 
where N1 and N2 are the lengths of the original sequences x[n] and h[n], 
respectively. 
Example: 
 Consider the sequences x[n] = [1, 2, 3] and h[n] = [4, 5]. 
1. Zero-padding: 
o Pad x[n] to [1, 2, 3, 0, 0] and h[n] to [4, 5, 0, 0]. 
2. Circular Convolution: 
o Perform circular convolution on the zero-padded sequences. The result 
will be 
[4, 13, 21, 15, 0]. 

3. Truncation: 
o Truncate the result to [4, 13, 21, 15]. 
 This result is the same as the linear convolution of x[n] and h[n]. 
Performing Circular Convolution Using Linear Convolution 
Method: 
1. Zero-Padding: 
o Pad both sequences x[n] and h[n] to a length of at least 2N-1, where N is 
the maximum length of the two sequences. 
2. Linear Convolution: 
o Perform linear convolution on the zero-padded sequences. 
3. Modulus Operation: 
o Apply the modulus operation to the indices of the linear convolution result, 
using the period N. This effectively wraps around the ends of the sequence, 
making it circular. 
Example: 
Using the same sequences as before, x[n] = [1, 2, 3] and h[n] = [4, 5]. 
1. Zero-padding: 
o Pad x[n] to [1, 2, 3, 0, 0] and h[n] to [4, 5, 0, 0]. 
2. Linear Convolution: 
o Perform linear convolution. The result will be [4, 13, 21, 15, 0]. 
3. Modulus Operation: 
o Apply the modulus operation to the indices: [4, 13, 21, 15, 0] becomes [4, 
13, 2, 15, 0].
# Observation:
## Linear using circular
![linear_using_circular_output](https://github.com/user-attachments/assets/99b6ebdf-0693-4c16-b94e-9a4416f867ba)
## Circular using linear
![circular_using_linear_output](https://github.com/user-attachments/assets/cda5d733-2281-4254-ba46-a3cab40565d7)
