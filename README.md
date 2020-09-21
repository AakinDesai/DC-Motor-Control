# DC Motor Control

## Summary

This project develops two different pieces of software that communicate with each other - PIC32 code for the motor driver and the client user interface that runs on the host computer.

<img src="Media/ControlSystem.png" width="800">

The PIC32 code (C Language) implements the control strategy (PID controller), consisting of a low-frequency position control loop and a nested high-frequency current control loop. The outer control loop runs at 200 Hz and the inner current control loop runs at 5 kHz. PWM is at 20 kHz.

### Results

**Current Control Error Plot:**

<img src="Media/CurrentControl.png" width="400">

**Step Trajectory Error Plot:**

<img src="Media/BestStepTraj.png" width="400">

**Cubic Trajectory Error Plot:**

<img src="Media/BestCubicTraj.png" width="400">
