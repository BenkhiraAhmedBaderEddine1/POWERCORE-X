## ⚡ POWERCORE-X — FPGA Power Electronics Controller

<p align="center">
  <img src="assets/powercore-circuit.svg" width="100%" alt="POWERCORE-X animated FPGA circuit illustration"/>
</p>

<p align="center">
  <strong>Intelligent Switching • Dead-Time Insertion • Fault Protection</strong>
</p>


 <div align="center">

<img src="https://capsule-render.vercel.app/api?type=rect&height=170&color=0:080D24,45:152B50,100:432A73&text=POWERCORE-X&fontColor=FFFFFF&fontSize=55&fontAlignY=45&desc=FPGA%20%7C%20POWER%20ELECTRONICS%20%7C%20DIGITAL%20CONTROL&descSize=13&descAlignY=72&animation=fadeIn" width="100%" />

<br/>

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=17&duration=3000&pause=900&color=42E8FF&center=true&vCenter=true&width=850&lines=ENGINEERING+THE+FUTURE+OF+DIGITAL+POWER+CONTROL;PRECISION+TIMING+%7C+FPGA+ARCHITECTURE;INTELLIGENT+SWITCHING+%7C+FAULT+PROTECTION;VHDL-2008+%7C+FINITE+STATE+MACHINES" alt="Animated project introduction" />

<br/><br/>

ADVANCED DIGITAL SYSTEMS ENGINEERING

Programmable Power Converter Gate-Signal Controller

<br/>

<img src="https://img.shields.io/badge/PROJECT-POWERCORE--X-42E8FF?style=for-the-badge&labelColor=10172D"/>
<img src="https://img.shields.io/badge/DOMAIN-FPGA%20ENGINEERING-9B7BFF?style=for-the-badge&labelColor=10172D"/>
<img src="https://img.shields.io/badge/LANGUAGE-VHDL--2008-FF9B45?style=for-the-badge&labelColor=10172D"/>
<img src="https://img.shields.io/badge/CONTROL-MOORE%20FSM-31D6A5?style=for-the-badge&labelColor=10172D"/>

<br/>

<img src="https://img.shields.io/badge/CLOCK-50%20MHz-42E8FF?style=flat-square"/>
<img src="https://img.shields.io/badge/DEAD--TIME-200%20ns-FF9B45?style=flat-square"/>
<img src="https://img.shields.io/badge/SWITCHING-4%20PHASES-9B7BFF?style=flat-square"/>
<img src="https://img.shields.io/badge/FAULT%20PROTECTION-ENABLED-31D6A5?style=flat-square"/>

<br/><br/>

ONE FPGA. PRECISE TIMING. INTELLIGENT POWER CONTROL.

Designing deterministic switching architectures with configurable timing, dead-time management, and safety-oriented digital logic.

<br/>

<a href="#-project-overview">PROJECT OVERVIEW</a>
  ◆  
<a href="#-system-architecture">ARCHITECTURE</a>
  ◆  
<a href="#-digital-control-engine">CONTROL ENGINE</a>
  ◆  
<a href="#-verification">VERIFICATION</a>
  ◆  
<a href="#-getting-started">GET STARTED</a>

<br/><br/>

<img src="https://capsule-render.vercel.app/api?type=rect&height=3&color=0:42E8FF,50:9B7BFF,100:FF9B45" width="100%"/>

</div>

<div align="center">

◈ THE ENGINEERING CONCEPT

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=14&duration=2500&pause=700&color=9B7BFF&center=true&vCenter=true&width=750&lines=FROM+DIGITAL+LOGIC+TO+POWER+CONVERSION;FROM+FINITE+STATE+MACHINES+TO+SAFE+SWITCHING;PRECISION+IS+NOT+OPTIONAL.+IT+IS+THE+DESIGN." />

</div>



Abstract

Power electronic converters constitute essential components of modern electrical and electronic systems, including renewable energy installations, electric vehicles, industrial motor drives, battery energy storage systems, and high-efficiency energy conversion applications.

The performance and reliability of these systems depend significantly on the accuracy, synchronization, and safety of the switching signals applied to semiconductor power devices.

This project presents POWERCORE-X, an FPGA-based digital control architecture designed to generate accurately timed complementary gate-control signals for power converter switching stages.

The proposed architecture is developed using VHDL-2008 and is based on a synchronous Moore Finite State Machine (FSM). It extends a conventional four-phase waveform generator through modular timing management, configurable dead-time insertion, output interlocking, fault detection, and latched shutdown mechanisms.

The reference architecture operates from a 50 MHz FPGA clock and implements a four-phase switching sequence with durations of 10 µs, 30 µs, 10 µs, and 50 µs.

The development methodology includes engineering requirements analysis, mathematical timing calculations, RTL architecture design, VHDL implementation, automated testbench development, functional simulation, and preparation for FPGA hardware implementation.

The project aims to establish a reusable and extensible digital switching controller that demonstrates the application of FPGA technology to deterministic and safety-oriented power electronics control.

Keywords: FPGA, VHDL-2008, Embedded Digital Control, Power Electronics, Moore FSM, Gate Signal Generation, Dead-Time Insertion, Fault Protection, RTL Design, Hardware Verification.

<h2 align="center">02 │ INTRODUCTION</h2>

<p align="center">
  <strong>━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━</strong>
</p>

2.1 Background

The increasing demand for efficient, reliable, and controllable electrical energy conversion systems has made power electronics one of the most important areas of modern electrical engineering.

Power electronic converters are widely employed in:

Renewable energy generation systems.

Electric vehicles and charging infrastructure.

Industrial motor drives.

Battery management and energy storage.

Uninterruptible power supplies.

Industrial automation.

High-frequency switching power supplies.

A fundamental component of these systems is the switching control mechanism.

Semiconductor devices such as Metal-Oxide-Semiconductor Field-Effect Transistors (MOSFETs) and Insulated-Gate Bipolar Transistors (IGBTs) require carefully coordinated control signals to determine their conduction and blocking states.

Incorrect switching timing can cause undesirable electrical behavior, increased switching losses, and potentially destructive short-circuit conditions.

For this reason, digital switching controllers must provide predictable timing, coordinated output transitions, and appropriate protection mechanisms.

2.2 FPGA Technology in Digital Control

Field-Programmable Gate Arrays (FPGAs) offer a powerful platform for implementing deterministic digital control systems.

Unlike conventional software-based controllers, FPGA devices implement digital logic directly in configurable hardware resources.

Their main characteristics include:

Parallel hardware execution.

Deterministic logic operation.

Clock-cycle-level timing control.

Reconfigurable digital architecture.

Hardware implementation of state machines.

Dedicated counters and registers.

Flexible input/output interfaces.

FPGAs are therefore suitable for applications requiring precise digital timing and coordinated switching behavior.

2.3 Project Introduction

POWERCORE-X investigates the design of an FPGA-based digital controller for generating complementary switching signals.

The project originates from a conventional four-state Moore FSM waveform generator.

The original architecture produces two non-overlapping control signals according to a predefined switching sequence.

The proposed POWERCORE-X architecture extends this baseline through additional digital control and protection functions:

Configurable switching intervals.

Dead-time insertion.

Output mutual-exclusion logic.

Enable and reset management.

Fault detection.

Fault-state latching.

Modular RTL implementation.

Automated functional verification.

The objective is to move from a basic waveform generator toward a structured digital switching controller suitable for further engineering investigation.

<h2 align="center">03 │ PROBLEM STATEMENT</h2>

<p align="center">
  <strong>━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━</strong>
</p>

3.1 Engineering Problem

A basic FSM-based waveform generator can produce predetermined switching sequences. However, practical power converter control requires additional mechanisms to coordinate switching transitions and respond to abnormal conditions.

The main engineering challenges include:

Accurate generation of switching intervals.

Prevention of simultaneous activation of complementary outputs.

Controlled insertion of dead-time.

Reliable enable and reset behavior.

Detection of fault conditions.

Prevention of unintended automatic restart.

Verification of normal and abnormal operating scenarios.

3.2 Central Research Question

How can an FPGA-based digital controller be designed to generate accurately timed complementary switching signals while integrating configurable timing, dead-time management, output interlocking, and fault protection?

3.3 Proposed Solution

POWERCORE-X addresses this problem through a modular VHDL architecture based on synchronous digital logic.

The proposed system integrates a clock-driven timing manager, a Moore finite state machine, a programmable dead-time mechanism, a fault-management block, and complementary output logic.



