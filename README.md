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
Am=5.9;
fm=517;
Ac=11.8;
fc=5170;
fs=51700;
t=0:1/fs:2/fm;
m=Am*cos(2*3.14*fm*t);
subplot(3,1,1);
plot(t,m);
c=Ac*cos(2*3.14*fc*t);
subplot(3,1,2);
plot(t,c);
s=(Ac+m).*cos(2*3.14*fc*t);
subplot(3,1,3);
plot(t,s);

```

# Output Waveform:

<img width="1620" height="987" alt="image" src="https://github.com/user-attachments/assets/82e4b53d-f8fa-4f00-bfd4-f11a34572d65" />


Tabular Column:

![WhatsApp Image 2025-11-28 at 21 10 58_10f383e3](https://github.com/user-attachments/assets/5770eb85-276c-4d5b-b851-e82c059ed0e0)


# Algorithm:

Initialize Parameters: Set the values for carrier frequency, message frequency, and sampling frequency.
Generate Time Axis: Create a time vector for the signal duration.
Generate Message Signal: Define the message signal as a cosine wave.
Generate Carrier Signal: Define the carrier signal as a cosine wave.
Modulate Signal: Apply the AM formula to obtain the modulated signal.
Plot the Signals: Use Matplotlib to plot the message signal, carrier signal, and modulated signal.

# Result:

The message signal, carrier signal, and amplitude modulated (AM) signal will be displayed in separate plots. Thus AM is implemented using numPy and Matplotlib.
