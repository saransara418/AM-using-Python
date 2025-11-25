# AM USING PYTHON:

# Aim:

To implement and analyze amplitude modulation (AM) using Python's NumPy and Matplotlib libraries.

# Apparatus Required:

Software: Python with NumPy and Matplotlib libraries Hardware: Personal Computer

# Theory:

Amplitude Modulation (AM) is a technique used in electronic communication, primarily for transmitting information via a radio carrier wave. In AM, the amplitude of the carrier wave is varied in proportion to that of the message signal. The general form of an AM signal is:
![WhatsApp Image 2025-10-30 at 08 57 27_00c78055](https://github.com/user-attachments/assets/e5172107-622e-4b03-a3ed-6623574ba056)

# Program:
```
import numpy as np
import matplotlib.pyplot as plt

Am = 2.8
fm = 174
Ac = 5.6
fc = 1740
fs = 17400

t = np.arange(0, 2/fm, 1/fs)
m = Am * np.cos(2 * np.pi * fm * t)
plt.subplot(3, 1, 1)
plt.plot(t, m)
c = Ac * np.cos(2 * np.pi * fc * t)
plt.subplot(3, 1, 2)
plt.plot(t, c)
s = (Ac + m) * np.cos(2 * np.pi * fc * t)
plt.subplot(3, 1, 3)
plt.plot(t, s)
```

# Output Waveform:

<img width="1920" height="1080" alt="Screenshot (125)" src="https://github.com/user-attachments/assets/1ae41b2a-648b-42f4-a4bd-df86d62a2be1" />

Tabular Column:

![AM PYTHON](https://github.com/user-attachments/assets/a5e89c8e-28e3-4839-a2a7-441b64a75b72)

# Algorithm:

Initialize Parameters: Set the values for carrier frequency, message frequency, and sampling frequency.
Generate Time Axis: Create a time vector for the signal duration.
Generate Message Signal: Define the message signal as a cosine wave.
Generate Carrier Signal: Define the carrier signal as a cosine wave.
Modulate Signal: Apply the AM formula to obtain the modulated signal.
Plot the Signals: Use Matplotlib to plot the message signal, carrier signal, and modulated signal.

# Result:

The message signal, carrier signal, and amplitude modulated (AM) signal will be displayed in separate plots. Thus AM is implemented using numPy and Matplotlib.
