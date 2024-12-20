# Aim:
1.DFT using inbuilt function and without using inbuilt function. Also plot magnitude and phase 
plot of DFT
2.IDFT using inbuilt function and without using inbuilt function.
# Theory:
Discrete Fourier Transform (DFT)
 The Discrete Fourier Transform (DFT) is a mathematical transformation used to analyze 
the frequency content of discrete signals. For a sequence x[n] of length N, the DFT is defined 
as:
𝑿[𝒌] = ∑ 𝒙[𝒏]
𝑵
𝒏=𝟎
⋅ 𝒆
−𝒋
𝟐𝝅
𝑵
𝒏𝒌
, 𝒌 = 𝟎, 𝟏, 𝟐, . . . , 𝑵 −1
• X[k] is the DFT of the sequence x[n].
• The exponential factor represents 𝒆
−𝒋
𝟐𝝅
𝑵
𝒏𝒌 the complex sinusoidal basis functions.
• The DFT maps the time-domain signal into the frequency domain.
Inverse Discrete Fourier Transform (IDFT)Method:
 The Inverse Discrete Fourier Transform (IDFT) is used to convert a frequency-domain 
sequence X[k] back into its time-domain sequence x[n]. The IDFT is defined as:
𝒙[𝒏] =
𝟏
𝑵
∑ 𝑿[𝒌]
𝑵
𝒌=𝟎
⋅ 𝒆
𝒋
𝟐𝝅
𝑵
𝒏𝒌
, 𝒏 = 𝟎, 𝟏, 𝟐, . . . , 𝑵 −1
• The IDFT takes the frequency components X[k] and reconstructs the original sequence 
x[n].
• The exponential factor 𝒆
𝒋
𝟐𝝅
𝑵
𝒏𝒌 is the inverse of the DFT’s complex sinusoidal basis 
functions
.
Application
• Spectrum (Analysis)
• Filtering
• Compression
• Modulation
• Convolution
• Demodulation

• Equalization
• Restoration
• Detection
• Estimation

# Observation:
## DFT
![output6](https://github.com/user-attachments/assets/31429692-fe32-4836-8ac7-dd56398462d4)


## IDFT
![Screenshot 2024-11-09 183135](https://github.com/user-attachments/assets/e8c90765-f1db-41a4-9cf0-e26f6986d7b8)
