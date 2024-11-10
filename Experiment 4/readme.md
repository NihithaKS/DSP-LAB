# Aim:
To find circular convolution 
1. Using FFT and IFFT. 
2. Using Concentric Circle Method. 
3. Using Matrix Method.
# Theory:
Circular convolution is a mathematical operation that is like linear convolution 
but is performed in a periodic or circular manner. This is particularly useful in discretetime signal processing where signals are often represented as periodic sequences. 
 Mathematical Definition: 
 Given two periodic sequences x[n] and h[n], their circular convolution is define as:
 y[n] = (x[n] ⊛ h[n]) = ∑_{k=0} ^{N-1} x[k]h[(n-k) mod N] 
 Applications: 
• Discrete-Time Filtering: Circular convolution is used for filtering discretetime signals. 
• Digital Signal Processing: It's a fundamental operation in many digital signal 
processing algorithms. 
• Cyclic Convolution: In certain applications, such as cyclic prefix OFDM, 
circular convolution is used to simplify the implementation of linear 
convolution.
# Observation:
## Concentric circle method
![concentric_output](https://github.com/user-attachments/assets/e2325fd6-8ef9-448c-904b-e86a41500106)
## FFT and IFFT
![fftifft_output](https://github.com/user-attachments/assets/7386f381-e673-4094-bdd2-b2415d3c1626)
## Matrix mathod
![matrix_output](https://github.com/user-attachments/assets/9411c1ef-740d-4ae4-8681-bfeb8ceaa966)

