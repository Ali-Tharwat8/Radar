# Radar System Design & Signal Generation Project

This project involves the design and simulation of a pulsed radar system to detect objects and accurately measure their distance and velocity.

## System Overview

The radar operates at a **77 GHz** carrier frequency, utilizing 2,048 pulses to achieve a high target velocity resolution of under 0.5 m/s.

### Key System Parameters

* 
**Carrier Frequency ():** 77 GHz 


* 
**Pulse Repetition Interval (PRI):** 2 μs 


* 
**Pulse Width ():** 4.5 ns 


* 
**Signal-to-Noise Ratio (SNR):** -5 dB 


* 
**Max Unambiguous Range:** 299.8 m 


* 
**Max Unambiguous Velocity:** 486.7 m/s 



## Simulation Scenario

The simulation tracks two specific targets moving in opposite directions:

* 
**Target 1:** Located at **50m**, approaching at **-20 m/s**.


* 
**Target 2:** Located at **135m**, receding at **35 m/s**.



## Signal Analysis & Results

The system uses Doppler analysis and 2D FFT processing to isolate targets from the noise floor.

* 
**Range Performance:** Detected Target 1 at 50.01m and Target 2 at 135.03m.


* 
**Velocity Performance:** Estimated Target 1 velocity at -19.96 m/s and Target 2 at 35.17 m/s.


* 
**Visualization:** Range-Doppler maps and spectra provide a clear representation of target power and movement.



## Project Requirements

| Metric | Requirement | Result |
| --- | --- | --- |
| **Target Range Resolution** | < 0.75m | 0.675m 

 |
| **Target Velocity Resolution** | < 0.5m/s | ~0.47m/s 

 |
| **Max Unambiguous Range** | > 250m | 299.8m 

 |

**Authors:** Ali Tharwat and Abdulrhamn Jalal.
