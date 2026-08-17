<div align="center">

<img src="https://raw.githubusercontent.com/karimrayttu/karimrayttu/main/assets/banner.png" width="100%" alt="Karim Mahdi, ECE showcase: power electronics, embedded systems, PCB design. With portraits of Faraday, Tesla, Turing and Einstein.">

<br><br>

<a href="https://karimee.com"><img src="https://img.shields.io/badge/PORTFOLIO-21262d?style=for-the-badge&labelColor=21262d" alt="Portfolio"></a>
&nbsp;<a href="https://www.linkedin.com/in/karimrmahdi/"><img src="https://img.shields.io/badge/LINKEDIN-21262d?style=for-the-badge&labelColor=21262d" alt="LinkedIn"></a>
&nbsp;<a href="https://github.com/karimrayttu?tab=repositories"><img src="https://img.shields.io/badge/REPOSITORIES-21262d?style=for-the-badge&labelColor=21262d" alt="Repositories"></a>

<br><br>

<sub>This is my new GitHub account, where I showcase my work.</sub>

</div>

## What I do

I draw the schematic, lay out the board, bring it up, and prove it on the bench.

- **Power electronics.** DC-DC, gate drive, current sense, OCP/OVP/UVLO, reverse polarity.
- **Bare-metal firmware.** STM32 and MSP430, no HAL and no RTOS unless it earns its place.
- **Verification.** Every number in these repos is measured or simulated, and the method is written down next to it.

Right now I am widening the instrument coverage in [ece-tool-suite](https://github.com/karimrayttu/ece-tool-suite), so one session drives oscilloscopes, DMMs and spectrum analyzers across vendors rather than assuming a single SCPI dialect. Each family gets a capability profile, refined by model number where the vendor encodes it, and the interface renders only what the connected unit can actually do.

Ask me about protection circuits, SCPI bench automation, or why your gate drive is ringing.

<div align="center">
<br>
<img width="640" src="https://raw.githubusercontent.com/karimrayttu/karimrayttu/main/assets/scope.png" alt="A 200 microsecond per division capture with the channel's Vpp, Vmax and Vrms read back over SCPI">
<br>
<sub>Driving a scope over SCPI from <a href="https://github.com/karimrayttu/ece-tool-suite">ece-tool-suite</a>: 200 &#181;s/div, with the channel measurements read back off the instrument.</sub>
</div>

## Selected work

| Project | Result |
| :--- | :--- |
| **[bldc-predictive-maintenance](https://github.com/karimrayttu/bldc-predictive-maintenance)**<br><sub>Senior capstone</sub> | **99.63 %** held-out accuracy and **zero** false alarms over 7,189 healthy windows, from 60 runs recorded in one session. The classifier runs on the same STM32 that takes the measurement.<br><sub>C &#183; Python &#183; STM32</sub> |
| **[dc-protection-unit-40v](https://github.com/karimrayttu/dc-protection-unit-40v)** | A 40 V / 5 A P-FET disconnect on an analog trip path, **no firmware in the loop**, self-recovering. Documents where my own sense chain hits the ADC ceiling at rated current.<br><sub>LTspice &#183; Arduino &#183; Python</sub> |
| **[ece-tool-suite](https://github.com/karimrayttu/ece-tool-suite)** | Bench software that refuses to call a power stage sized until the netlist has been through SPICE. Drives scope, DMM, spectrum analyzer and supplies over SCPI/VISA.<br><sub>Python &#183; TypeScript &#183; Electron</sub> |
| **[mail-sorter-jetson](https://github.com/karimrayttu/mail-sorter-jetson)** | Reads handwritten addresses on a Jetson Orin, then a stepper drops each piece into the right bin. **Every piece routed correctly**, all of it resolved by ZIP.<br><sub>Python &#183; YOLO &#183; Jetson</sub> |
| **[autonomous-rover-msp430](https://github.com/karimrayttu/autonomous-rover-msp430)** | Beacon homing with obstacle avoidance, inductive metal detection, and an electromagnet on a belt slider. Bare-metal C, real-time state machine, three rails.<br><sub>C &#183; MSP430</sub> |

## Tools

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/karimrayttu/karimrayttu/main/assets/tools-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/karimrayttu/karimrayttu/main/assets/tools-light.svg">
  <img src="https://raw.githubusercontent.com/karimrayttu/karimrayttu/main/assets/tools-dark.svg" alt="Design and simulation: Altium Designer, KiCad, EAGLE, Fusion 360, LTspice, ngspice, MATLAB. Silicon and code: STM32, MSP430, ARM Cortex-M, FPGA, Jetson Orin, C, C++, Python, Rust, Verilog, VHDL. Bench: SCPI/VISA, oscilloscope, spectrum analyzer, LabVIEW, Arch and Ubuntu" width="100%">
</picture>

<div align="center">
<br>
<sub>Boards, firmware, and the measurements that prove they work.</sub>
</div>
