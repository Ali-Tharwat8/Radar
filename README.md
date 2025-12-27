# Pulse Doppler Radar System Simulation

A comprehensive simulation of a 77 GHz pulse Doppler radar system for target detection, range estimation, and velocity analysis using matched filtering and Doppler processing.

## Overview

This project implements a complete radar signal processing pipeline that simulates automotive radar systems commonly used in Advanced Driver Assistance Systems (ADAS). The simulation demonstrates target detection, range-Doppler mapping, and velocity estimation under realistic conditions including noise.

## System Parameters

| Parameter | Value | Description |
|-----------|-------|-------------|
| Carrier Frequency | 77 GHz | Operating frequency (automotive radar band) |
| PRI (Pulse Repetition Interval) | 2 μs | Time between consecutive pulses |
| Pulse Width | 4.5 ns | Duration of transmitted pulse |
| Sampling Points | 1,000,000 | Number of samples in simulation |
| SNR | -5 dB | Signal-to-Noise Ratio |

## Performance Specifications

The system meets the following requirements:

- **Maximum Unambiguous Range**: 299.8 m (requirement: > 250 m)
- **Maximum Unambiguous Velocity**: 486.7 m/s (realistic range: -100 to 100 m/s)
- **Range Resolution**: < 0.75 m
- **Velocity Resolution**: < 0.5 m/s
- **Number of Pulses**: 2048

## Features

### A) Signal Generation
- Pulse radar waveform generation
- Target scenario simulation with multiple targets
- Transmitted and received signal visualization
- Range-time plot generation

### B) Matched Filtering
- Noise addition to simulate realistic conditions
- Signal processing under low SNR conditions
- Pre-filtering signal analysis

### C) Doppler Analysis
- Velocity estimation using Doppler frequency shift
- Direction classification (approaching/receding)
- Doppler spectrum visualization
- High-accuracy target parameter extraction

### D) Range-Doppler Processing
- 2D Range-Doppler map generation
- Simultaneous range and velocity estimation
- Multi-target detection and separation

## Test Scenario Results

The system was tested with two targets:

| Target | Range | Velocity | Detection Accuracy |
|--------|-------|----------|-------------------|
| Target 1 | 50 m | -20 m/s (approaching) | Range: 50.01 m, Velocity: -19.96 m/s |
| Target 2 | 135 m | +35 m/s (receding) | Range: 135.03 m, Velocity: +35.17 m/s |

**Detection Error**: 
- Range error: < 0.03 m (< 0.02%)
- Velocity error: < 0.2 m/s (< 1%)

## Key Formulas

**Maximum Unambiguous Range:**
```
R_max = (C × PRI) / 2
```

**Maximum Unambiguous Velocity:**
```
v_max = (C × PRF) / (4 × F_c)
```

**Range Resolution:**
```
ΔR = (C × T_p) / 2
```

**Velocity Resolution:**
```
v_res = λ / (2 × N × PRI)
```

## Visualizations

The project generates the following plots:

1. **Transmitted/Received Signals**: Time-domain representation of radar pulses
2. **Range-Time Plot**: Target position over time
3. **Noisy Received Signal**: Signal characteristics under low SNR
4. **Doppler Spectrum**: Frequency domain analysis for velocity estimation
5. **Range-Doppler Map**: 2D visualization of target range and velocity

## Applications

- Automotive radar systems (ADAS, autonomous vehicles)
- Speed detection and traffic monitoring
- Range and velocity measurement
- Multi-target tracking
- Radar signal processing education
 Real-time processing implementation

## Contributors

This project was developed by:

- **Abdelrahman Jalal** - https://github.com/abdulrhman-dev
- **Ali Tharwat** - https://github.com/Ali-Tharwat8

Developed as part of a radar systems course/research project.

*77 GHz Automotive Radar Simulation - Target Detection & Velocity Estimation*
