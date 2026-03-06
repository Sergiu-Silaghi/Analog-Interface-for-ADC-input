# Analog-Interface-for-ADC-input
Design and practical implementation of an analog interface for ADC input, including theoretical analysis and experimental validation.

## Overview
This project presents the design and practical implementation of an **analog signal conditioning interface for an Analog-to-Digital Converter (ADC)**. The purpose of the system is to properly prepare an analog signal before it is sampled by the ADC, improving signal quality, amplitude range, and measurement accuracy.
The interface is composed of **four analog processing stages**, each responsible for conditioning the signal before it reaches the ADC input.

---

## System Architecture

The analog interface consists of the following stages:

1. **Instrumentation Amplifier**
2. **Analog Filter**
3. **Programmable Gain Amplifier (PGA)**
4. **Precision Rectifier**

Signal flow:
Input Signal → Instrumentation Amplifier → Filter → PGA → Precision Rectifier → ADC Input

Each stage performs a specific signal conditioning function to ensure optimal compatibility with the ADC.

---

## Stage Description

### 1. Instrumentation Amplifier
The first stage is an **instrumentation amplifier**, designed to amplify low-level differential signals while rejecting common-mode noise.

Main functions:
- High input impedance
- High Common Mode Rejection Ratio (CMRR)
- Accurate amplification of small signals
- Noise reduction

This stage is particularly useful for signals coming from sensors.

---

### 2. Analog Filter
The second stage is an **analog filter**, used to limit the bandwidth of the signal before it is digitized.

Main purposes:
- Removal of high-frequency noise
- Signal smoothing
- Anti-aliasing preparation before ADC sampling

Depending on the design, the filter can be implemented as:
- Low-pass filter
- Active filter using operational amplifiers

---

### 3. Programmable Gain Amplifier (PGA)
The third stage is a **Programmable Gain Amplifier**, which allows the amplification factor to be adjusted depending on the amplitude of the input signal.

Advantages:
- Adaptation to different signal ranges
- Improved ADC resolution
- Flexible signal conditioning

The gain can be selected using different resistor configurations and switching elements.

---

### 4. Precision Rectifier
The final stage is a **precision rectifier**, designed to rectify the signal without the voltage drop associated with standard diode rectifiers.

Main features:
- Accurate rectification of signals
- No significant diode threshold voltage error
- Improved signal accuracy before ADC conversion

This stage ensures that the ADC receives a properly conditioned signal.

---

## Practical Implementation
In addition to the theoretical design, the project includes a **practical hardware implementation**.

The implementation involves:
- Circuit schematic design
- Component selection
- Breadboard assembly
- Experimental testing and signal measurements

Measurements were performed to verify:
- Signal amplification
- Filter response
- Gain programmability
- Rectifier performance

---

## Applications
Such an analog interface can be used in various applications, including:

- Sensor signal conditioning
- Data acquisition systems
- Measurement instrumentation
- Biomedical signal processing
- Industrial monitoring systems

---

## Tools and Components
Tools and components used in the project:

- Operational amplifiers
- Resistors and capacitors
- Analog switches and gain control circuits
- Oscilloscope
- Signal generator
- Breadboard
- Scopy software designed by Analog Devices

---

## Learning Objectives
This project helps develop practical and theoretical knowledge in:

- Analog circuit design
- Signal conditioning
- Operational amplifier applications
- ADC interfacing
- Analog filtering techniques
- Practical electronic circuit implementation

---

## Author
University project developed as part of coursework related to **Systems with Analog Integrated Circuits**.
