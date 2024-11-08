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

Observation:
1.DFT
enter sequence:[1 1 1 0]
enter the N point:8
X
  Columns 1 through 7
   3.0000 + 0.0000i   1.7071 - 1.7071i   0.0000 - 1.0000i   0.2929 + 0.2929i   1.0000 + 0.0000i   0.2929 - 0.2929i  -0.0000 + 1.0000i
  Column 8
   1.7071 + 1.7071i
round(X)
  Columns 1 through 7
   3.0000 + 0.0000i   2.0000 - 2.0000i   0.0000 - 1.0000i   0.0000 + 0.0000i   1.0000 + 0.0000i   0.0000 + 0.0000i   0.0000 + 1.0000i
  Column 8
   2.0000 + 2.0000i
fft
  Columns 1 through 7
   3.0000 + 0.0000i   1.7071 - 1.7071i   0.0000 - 1.0000i   0.2929 + 0.2929i   1.0000 + 0.0000i   0.2929 - 0.2929i   0.0000 + 1.0000i
  Column 8
   1.7071 + 1.7071i

2.IDFT
enter sequence: [3.0000 + 0.0000i   1.7071 - 1.7071i   0.0000 - 1.0000i   0.2929 + 0.2929i   1.0000 + 0.0000i   0.2929 - 0.2929i   0.0000 + 1.0000i]
enter the n point:8
x
   0.7866 - 0.2134i
   0.6982 - 0.0000i
   0.7866 + 0.2134i
  -0.0000 + 0.3018i
   0.2134 + 0.2134i
   0.3018 - 0.0000i
   0.2134 - 0.2134i
   0.0000 - 0.3018i

round(x)
     1
     1
     1
     0
     0
     0
     0
     0

ifft
  Columns 1 through 7

   0.7866 - 0.2134i   0.6982 + 0.0000i   0.7866 + 0.2134i   0.0000 + 0.3018i   0.2134 + 0.2134i   0.3018 + 0.0000i   0.2134 - 0.2134i 

  Column 8

   0.0000 - 0.3018i
