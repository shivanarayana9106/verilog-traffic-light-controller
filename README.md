# verilog-traffic-light-controller
Verilog implementation of a two-road Traffic Light Controller using a Finite State Machine (FSM). The design controls traffic signals for two directions with timed green, yellow, and red phases, and includes a comprehensive testbench for simulation and waveform verification.
# Traffic Light Controller using Verilog HDL
## Overview
This project implements a two-road Traffic Light Controller using Verilog HDL. The controller is designed using a Finite State Machine (FSM) to control the traffic signals at an intersection. It cycles through Green, Yellow, and Red lights for each road based on predefined timing intervals.

## Features
- Finite State Machine (FSM) based design
- Four traffic light states
- Counter-based timing control
- Asynchronous active-high reset
- Separate signals for Road A and Road B
- Verilog testbench for functional verification

## State Sequence

| State | Road A | Road B | Duration |
|-------|--------|--------|----------|
| S0 | Green | Red | 15 Clock Cycles |
| S1 | Yellow | Red | 8 Clock Cycles |
| S2 | Red | Green | 15 Clock Cycles |
| S3 | Red | Yellow | 8 Clock Cycles |
![Uploading image.png…]()

## Inputs
- `clk` : System Clock
- `reset` : Asynchronous Reset

## Outputs
- `a_red`
- `a_yellow`
- `a_green`
- `b_red`
- `b_yellow`
- `b_green`

## Files

```
rtl/
    trafficlight.v

testbench/
    trafficlight_tb.v
```

## Tools Used
- Verilog HDL
- Xilinx Vivado Simulator
- GitHub

## Learning Outcomes
- Finite State Machine Design
- Sequential Logic Design
- Counter Design
- Verilog HDL Coding
- Testbench Development
- Digital Circuit Simulation
