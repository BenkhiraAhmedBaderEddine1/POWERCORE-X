
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 520" width="1200" height="520">
  <defs>
    <linearGradient id="bg" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0%" stop-color="#050b1a"/>
      <stop offset="55%" stop-color="#101b36"/>
      <stop offset="100%" stop-color="#080d20"/>
    </linearGradient>

  
  <linearGradient id="chip" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0%" stop-color="#182e52"/>
      <stop offset="100%" stop-color="#091326"/>
    </linearGradient>

  <linearGradient id="electric">
      <stop offset="0%" stop-color="#00eaff"/>
      <stop offset="50%" stop-color="#7b61ff"/>
      <stop offset="100%" stop-color="#00eaff"/>
    </linearGradient>
    <filter id="glow">
      <feGaussianBlur stdDeviation="5" result="blur"/>
      <feMerge>
        <feMergeNode in="blur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>
    <pattern id="grid" width="40" height="40" patternUnits="userSpaceOnUse">
      <path d="M40 0H0V40" fill="none" stroke="#28436b" stroke-width="0.7" opacity=".35"/>
    </pattern>
  </defs>

  <!-- Background -->
  <rect width="1200" height="520" rx="24" fill="url(#bg)"/>
  <rect width="1200" height="520" rx="24" fill="url(#grid)"/>

  <!-- Decorative circuit traces -->
  <g fill="none" stroke="#176b9b" stroke-width="2" opacity=".65">
    <path d="M0 110H170V180H330"/>
    <path d="M0 390H200V330H350"/>
    <path d="M1200 110H1030V180H870"/>
    <path d="M1200 390H1000V330H850"/>
    <path d="M600 0V75"/>
    <path d="M600 445V520"/>
    <path d="M180 0V70H280"/>
    <path d="M1020 520V440H920"/>
  </g>

  <!-- Circuit connection points -->
  <g fill="#00eaff" filter="url(#glow)">
    <circle cx="170" cy="110" r="4"/>
    <circle cx="200" cy="390" r="4"/>
    <circle cx="1030" cy="110" r="4"/>
    <circle cx="1000" cy="390" r="4"/>
    <circle cx="600" cy="75" r="4"/>
    <circle cx="600" cy="445" r="4"/>
  </g>

  <!-- Left chip -->
  <g transform="translate(175 175)">
    <rect x="0" y="0" width="190" height="155" rx="14"
          fill="url(#chip)" stroke="#00cfff" stroke-width="2"/>
    <rect x="18" y="18" width="154" height="119" rx="8"
          fill="#071326" stroke="#28618b"/>
    <g stroke="#00dfff" stroke-width="4">
      <path d="M25 -12V0 M55 -12V0 M85 -12V0 M115 -12V0 M145 -12V0"/>
      <path d="M25 155V167 M55 155V167 M85 155V167 M115 155V167 M145 155V167"/>
      <path d="M-12 30H0 M-12 65H0 M-12 100H0 M190 30H202 M190 65H202 M190 100H202"/>
    </g>
    <text x="95" y="65" text-anchor="middle" fill="#00eaff"
          font-size="20" font-weight="bold" font-family="monospace">FPGA</text>
    <text x="95" y="91" text-anchor="middle" fill="#8baacb"
          font-size="12" font-family="monospace">CONTROL LOGIC</text>
    <circle cx="95" cy="112" r="5" fill="#00eaff" filter="url(#glow)">
      <animate attributeName="opacity" values=".25;1;.25" dur="1.5s" repeatCount="indefinite"/>
    </circle>
  </g>

  <!-- Central processor -->
  <g transform="translate(465 125)">
    <rect x="0" y="0" width="270" height="220" rx="20"
          fill="url(#chip)" stroke="#8b6cff" stroke-width="2.5"
          filter="url(#glow)"/>
    <rect x="22" y="22" width="226" height="176" rx="12"
          fill="#071326" stroke="#4654a5" stroke-width="1.5"/>
    <g stroke="#8b6cff" stroke-width="5">
      <path d="M35 -14V0 M75 -14V0 M115 -14V0 M155 -14V0 M195 -14V0 M235 -14V0"/>
      <path d="M35 220V234 M75 220V234 M115 220V234 M155 220V234 M195 220V234 M235 220V234"/>
      <path d="M-14 35H0 M-14 75H0 M-14 115H0 M-14 155H0 M-14 195H0"/>
      <path d="M270 35H284 M270 75H284 M270 115H284 M270 155H284 M270 195H284"/>
    </g>
    <text x="135" y="82" text-anchor="middle" fill="#ffffff"
          font-size="27" font-weight="bold" font-family="monospace">POWERCORE-X</text>
    <text x="135" y="112" text-anchor="middle" fill="#00eaff"
          font-size="15" font-family="monospace">VHDL • FPGA</text>
    <path d="M65 140H205 M65 155H205" stroke="#294a78" stroke-width="2"/>
    <text x="135" y="181" text-anchor="middle" fill="#9b8aff"
          font-size="13" font-family="monospace">50 MHz • FSM</text>
  </g>

  <!-- Right power converter chip -->
  <g transform="translate(835 175)">
    <rect x="0" y="0" width="190" height="155" rx="14"
          fill="url(#chip)" stroke="#ff9c42" stroke-width="2"/>
    <rect x="18" y="18" width="154" height="119" rx="8"
          fill="#071326" stroke="#80512f"/>
    <g stroke="#ff9c42" stroke-width="4">
      <path d="M25 -12V0 M55 -12V0 M85 -12V0 M115 -12V0 M145 -12V0"/>
      <path d="M25 155V167 M55 155V167 M85 155V167 M115 155V167 M145 155V167"/>
      <path d="M-12 30H0 M-12 65H0 M-12 100H0 M190 30H202 M190 65H202 M190 100H202"/>
    </g>
    <text x="95" y="65" text-anchor="middle" fill="#ffb45e"
          font-size="19" font-weight="bold" font-family="monospace">POWER</text>
    <text x="95" y="91" text-anchor="middle" fill="#c6a68a"
          font-size="12" font-family="monospace">GATE DRIVER</text>
    <circle cx="95" cy="112" r="5" fill="#ff9c42" filter="url(#glow)">
      <animate attributeName="opacity" values="1;.2;1" dur="1.2s" repeatCount="indefinite"/>
    </circle>
  </g>

  <!-- Animated signal paths -->
  <g fill="none" stroke="#00dfff" stroke-width="2.5" opacity=".8">
    <path id="leftPath" d="M365 252H465"/>
    <path id="rightPath" d="M735 252H835"/>
    <path d="M365 285H430V365H600V345" stroke="#8b6cff"/>
    <path d="M835 285H770V365H600" stroke="#ff9c42"/>
  </g>

  <g filter="url(#glow)">
    <circle r="5" fill="#00eaff">
      <animateMotion dur="1.8s" repeatCount="indefinite">
        <mpath href="#leftPath"/>
      </animateMotion>
    </circle>
    <circle r="5" fill="#ffffff">
      <animateMotion dur="1.8s" repeatCount="indefinite" begin=".9s">
        <mpath href="#rightPath"/>
      </animateMotion>
    </circle>
    <circle r="4" fill="#a58bff">
      <animateMotion dur="2.4s" repeatCount="indefinite">
        <mpath href="#leftPath"/>
      </animateMotion>
    </circle>
  </g>

  <!-- Bottom signal waveform -->
  <g transform="translate(390 405)" fill="none" stroke="#00eaff" stroke-width="2.5">
    <path d="M0 40H45V10H90V40H135V10H180V40H225V10H270V40H315V10H360V40H405"/>
    <path d="M0 53H405" stroke="#385477" stroke-width="1" opacity=".6"/>
  </g>

  <text x="600" y="492" text-anchor="middle" fill="#6f94bb"
        font-size="12" letter-spacing="4" font-family="monospace">
    INTELLIGENT POWER ELECTRONICS CONTROL
  </text>

  <!-- Scanning light -->
  <rect x="0" y="0" width="1200" height="3" fill="#00eaff" opacity=".7">
    <animate attributeName="y" values="0;517;0" dur="7s" repeatCount="indefinite"/>
  </rect>
</svg>




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
