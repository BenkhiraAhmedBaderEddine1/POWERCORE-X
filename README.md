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

