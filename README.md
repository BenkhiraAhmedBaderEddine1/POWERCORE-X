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

⚡ PROJECT OVERVIEW

POWERCORE-X is an advanced FPGA-based digital control architecture developed to generate precisely timed complementary gate-control signals for power converter switching applications.

Built using VHDL-2008, the system combines finite state machine control, programmable timing counters, configurable dead-time insertion, output interlocking, and latched fault protection.

The architecture evolves from a conventional four-phase Moore FSM waveform generator into a modular and extensible digital switching controller.

CORE ENGINEERING PARAMETERS


CORE ENGINEERING PARAMETERS

Parameter

Specification

Project Architecture

FPGA-Based Digital Controller

Hardware Clock

50 MHz

Clock Period

20 ns

Control Architecture

Moore Finite State Machine

Hardware Description Language

VHDL-2008

Switching Intervals

10 / 30 / 10 / 50 µs

Configurable Dead-Time

200 ns

Protection Mechanism

Fault Latching

Output Architecture

Complementary Digital Signals

<div align="center">

◈ THE FOUR-PHASE SWITCHING ENGINE

100 µs Reference Switching Sequence

<img src="https://img.shields.io/badge/PHASE_01-10_%CE%BCs-42E8FF?style=for-the-badge"/>
<img src="https://img.shields.io/badge/PHASE_02-30_%CE%BCs-9B7BFF?style=for-the-badge"/>
<img src="https://img.shields.io/badge/PHASE_03-10_%CE%BCs-42E8FF?style=for-the-badge"/>
<img src="https://img.shields.io/badge/PHASE_04-50_%CE%BCs-FF9B45?style=for-the-badge"/>

</div>

DIGITAL SWITCHING SEQUENCE

TIME       0       10              40      50                      100 µs
           |--------|---------------|-------|------------------------|

SIG1       ████████                 ████████
           HIGH                     HIGH

SIG2               ███████████████         ████████████████████████
                   HIGH                     HIGH

STATE      PHASE_1  PHASE_2         PHASE_3 PHASE_4


The reference sequence above represents the original active switching intervals. In the enhanced architecture, dead-time intervals are inserted between transitions.

<div align="center">

◈ SYSTEM DESIGN PHILOSOPHY

<img src="https://img.shields.io/badge/01-TIMING%20PRECISION-42E8FF?style=for-the-badge"/>
<img src="https://img.shields.io/badge/02-SAFE%20SWITCHING-9B7BFF?style=for-the-badge"/>
<img src="https://img.shields.io/badge/03-FAULT%20MANAGEMENT-FF9B45?style=for-the-badge"/>

A modular architecture. A deterministic switching engine. A safety-oriented design.

</div>

🧬 SYSTEM ARCHITECTURE

                ┌──────────────────────┐
                │    50 MHz FPGA CLK   │
                └──────────┬───────────┘
                           │
                ┌──────────▼───────────┐
                │   TIMING MANAGER     │
                │  Counters & Timers   │
                └──────────┬───────────┘
                           │
                ┌──────────▼───────────┐
                │     MOORE FSM        │
                │  Four-Phase Control  │
                └──────────┬───────────┘
                           │
                ┌──────────▼───────────┐
                │    DEAD-TIME UNIT    │
                │   200 ns Reference   │
                └──────────┬───────────┘
                           │
                ┌──────────▼───────────┐
                │   FAULT MANAGEMENT   │
                │    Output Interlock  │
                └──────────┬───────────┘
                           │
                   ┌───────┴───────┐
                   │               │
             ┌─────▼─────┐   ┌─────▼─────┐
             │   SIG1    │   │   SIG2    │
             │  GATE A   │   │  GATE B   │
             └───────────┘   └───────────┘

🛡️ SAFETY-FIRST DIGITAL CONTROL

The primary digital safety invariant is:

[
Sig1 \land Sig2 = 0
]

The architecture is designed to ensure that complementary outputs are never simultaneously asserted.

Additional mechanisms include:

Configurable dead-time insertion.

Output mutual-exclusion logic.

Fault detection and latching.

Controlled activation and reset.

Safe output shutdown.

Engineering note: Digital interlocking is not a substitute for independent gate-driver protection, electrical isolation, and hardware overcurrent protection.

