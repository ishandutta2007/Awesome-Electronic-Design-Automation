# Awesome-Electronic-Design-Automation

## Top Electronic Design Automation (EDA) Platforms Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on IC Design, PCB Layout, Analog Simulation & Open-Silicon Flows*  

**Last updated: September 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Electronic Design Automation (EDA)**. These tools help chip designers, PCB engineers, and hardware teams create, simulate, verify, and manufacture electronic circuits — from custom silicon to production PCBs.



**Examples** include Cadence Virtuoso, Synopsys Fusion Compiler, Siemens EDA Xpedition, Altium 365, Zuken CR-8000, Silvaco SmartSpice, Keysight ADS, Ansys RedHawk, EasyEDA Pro, and Aldec Riviera-PRO (the category leaders).



**Open-source emphasis**: The open-source EDA ecosystem has matured dramatically. With **SkyWater SKY130**, **GlobalFoundries GF180MCU**, and **IHP SG13G2** open PDKs, combined with tools like **Yosys**, **OpenROAD**, **Xschem**, **Magic**, and **KLayout**, complete analog and digital IC design flows can now run entirely on open-source software. **KiCad** leads PCB design, with **LibrePCB**, **Horizon EDA**, and **atopile** offering modern alternatives. This section documents every major active project across the full design stack.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents



- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[Cadence Virtuoso](https://www.cadence.com/)**

  Industry-standard custom IC design platform for analog, mixed-signal, and RF circuits. Provides schematic capture, simulation, layout, and full custom design flows. Used by virtually all major semiconductor companies.



- **[Synopsys Fusion Compiler](https://www.synopsys.com/)**

  RTL-to-GDSII implementation platform combining synthesis, place-and-route, and optimization. The dominant digital IC implementation solution for advanced nodes.



- **[Siemens EDA Xpedition](https://eda.sw.siemens.com/)**

  Enterprise PCB design platform for complex multi-board systems. Provides schematic capture, layout, signal integrity, and manufacturing preparation.



- **[Altium 365](https://www.altium.com/)**

  Cloud-connected PCB design platform. Provides schematic capture, PCB layout, 3D visualization, and collaboration features with browser-based access.



- **[Zuken CR-8000](https://www.zuken.com/)**

  PCB and multi-board design platform for enterprise electronics. Provides schematic, layout, and manufacturing preparation for complex systems.



- **[Silvaco SmartSpice](https://silvaco.com/)**

  Analog and mixed-signal circuit simulator for IC design. Provides accurate SPICE modeling and verification for custom circuits.



- **[Keysight ADS](https://www.keysight.com/)**

  Advanced Design System for RF, microwave, and high-speed digital design. Provides circuit simulation, electromagnetic analysis, and system-level design.



- **[Ansys RedHawk](https://www.ansys.com/)**

  Power integrity and reliability analysis platform for ICs. Analyzes IR drop, electromigration, and thermal effects in power delivery networks.



- **[EasyEDA Pro](https://easyeda.com/)**

  Cloud-based PCB design platform with integrated component library and manufacturing. Popular with hobbyists and small teams.



- **[Aldec Riviera-PRO](https://www.aldec.com/)**

  HDL simulation and verification platform for FPGA and ASIC design. Supports VHDL, Verilog, SystemVerilog, and SystemC.



## Open-Source GitHub Projects



### Digital IC Design (RTL to GDSII)



- **[Yosys](https://github.com/YosysHQ/yosys)**

  Open-source RTL synthesis framework. Converts Verilog RTL to gate-level netlists for FPGA and ASIC flows. The foundation of the open-source digital IC design toolchain, with a GHDL plugin enabling VHDL synthesis . **ISC License**.



- **[OpenROAD](https://github.com/The-OpenROAD-Project/OpenROAD)**

  Complete RTL-to-GDSII flow with place-and-route, static timing analysis, and power analysis. Integrated with PDNSim for static IR drop analysis in power delivery networks . The core of the OpenLane automated flow . **Apache-2.0**.



- **[OpenLane](https://github.com/The-OpenROAD-Project/OpenLane)**

  Automated digital ASIC design flow from RTL to GDSII. Originally initiated by Google and SkyWater to enable open-source chip design using the SKY130 PDK. Now supports multiple open PDKs including GF180MCU and IHP SG13G2 .



- **[OpenSTA](https://github.com/parallaxsw/OpenSTA)**

  Static timing analysis engine for gate-level netlists. Used within the OpenROAD flow for timing signoff . **GPL-3.0**.



### Analog & Mixed-Signal IC Design



- **[Xschem](https://github.com/StefanSchippers/xschem)**

  Schematic capture editor for analog and mixed-signal circuit design. Lightweight, fast, and designed for hierarchical designs. The schematic entry tool of choice in open-source analog flows . **GPL-2.0**.



- **[Ngspice](https://github.com/ngspice/ngspice)**

  The leading open-source mixed-level/mixed-signal circuit simulator. Successor to Berkeley SPICE 3f5, incorporating Xspice and Cider models. Supports nonlinear DC, transient, and linear AC analyses, with mixed-signal simulation by co-simulating with Verilog (via Verilator/Icarus) or VHDL (via GHDL) . Integrated into KiCad for built-in SPICE simulation . **BSD-3-Clause**.



- **[Xyce](https://github.com/Xyce/Xyce)**

  SPICE-compatible simulator from Sandia National Laboratories, designed for large-scale parallel circuit simulation. Used for full transistor-level simulation sign-off in open-source analog flows .



- **[Magic VLSI](https://github.com/RTimothyEdwards/magic)**

  Layout editor for custom IC design. Provides interactive layout editing, DRC, extraction, and LVS capabilities. Part of the open-source analog design flow for custom block layout .



- **[KLayout](https://github.com/KLayout/klayout)**

  High-performance layout viewer and editor. Provides DRC, LVS, and parasitic extraction. Extensible via Python and Ruby APIs. The standard layout verification tool in open-source IC flows .



### PCB Design



- **[KiCad](https://gitlab.com/kicad/code/kicad)**

  The leading open-source EDA suite for schematic capture and PCB layout. Used by hobbyists and professionals worldwide. Features hierarchical schematics, up to 32 copper layers, push-and-shove router, differential pair routing, 3D viewer with STEP support, Python scripting API, and integrated Ngspice simulation . CERN has contributed over 1,400 hours of developer time to KiCad, and it joined the Linux Foundation in 2019 . **GPLv3**.



- **[LibrePCB](https://github.com/LibrePCB/LibrePCB)**

  Modern, intuitive open-source EDA suite for schematic and PCB layout. Features a centralized library manager, design rule checks, multi-platform support, and open file formats. Built with C++ and Qt . **GPLv3**.



- **[Horizon EDA](https://github.com/carrotIndustries/horizon)**

  Free EDA package for schematic capture and PCB design. Focused on a modern, extensible architecture .



- **[atopile](https://github.com/atopile/atopile)**

  Language and toolchain to describe electronic circuit boards with code. Replaces point-and-click schematic entry with software development workflows including reuse, validation, and automation. Built with Python . **BSD**.



### PCB Analysis & Verification



- **[circuitcore](https://github.com/UnsignedChad/circuitcore)**

  PCB analysis toolkit with four integrated tools: **pdnkit** (power integrity — static IR drop, Z(f) cavity model, decap optimization, SPICE export), **sikit** (signal integrity — trace impedance, S-parameters, eye diagrams, IBIS/IBIS-AMI parsing), **emikit** (EMI/radiated emissions), and **mpkit** (multiphysics — thermal, elasticity). Parses `.kicad_pcb` files into a canonical board model. C++23, Qt6, Eigen, SuiteSparse, optional VTK 9 . **GPL-3.0**.



- **[OpenEMS](https://github.com/thliebig/openEMS)**

  Electromagnetic field solver for signal integrity and power integrity simulation of PCB designs. Uses FDTD method. Works with Octave/Python scripting and KiCad export macros .



- **[OpenFASOC](https://github.com/idea-fasoc/OpenFASOC)**

  Open-source analog layout generation. Includes **glayout**, a set of PDK-agnostic building blocks for programmatic analog circuit construction in Python .



### HDL Simulation & Verification



- **[Verilator](https://github.com/verilator/verilator)**

  Fast Verilog/SystemVerilog simulator. Compiles HDL to optimized C++/SystemC for cycle-accurate simulation. The fastest open-source Verilog simulator, widely used in digital design verification .



- **[Icarus Verilog](https://github.com/steveicarus/iverilog)**

  Verilog simulation and synthesis tool. Supports Verilog-2005 and experimental SystemVerilog. Used for digital simulation in open-source ASIC flows .



- **[GHDL](https://github.com/ghdl/ghdl)**

  Complete VHDL simulator with synthesis capabilities. Supports VHDL-1987 through VHDL-2019, PSL assertions, and co-simulation via VPI/VHPIDIRECT. The standard open-source VHDL simulator .



- **[NVC](https://github.com/nickg/nvc)**

  VHDL compiler and simulator with experimental Verilog support. Recently became the first "true" open-source mixed-language simulator, compiling Verilog and VHDL sources together sharing a common simulation kernel without source translation .



- **[Cocotb](https://github.com/cocotb/cocotb)**

  Coroutine-based co-simulation testbench environment for verifying VHDL/Verilog RTL using Python. Enables Python-based verification without HDL testbenches. Used in open-source ASIC flows for digital test benches .



### Open PDKs (Process Design Kits)



- **[SkyWater SKY130 PDK](https://github.com/google/skywater-pdk)**

  130nm open-source production PDK developed by Google and SkyWater Technology. Enables fully open-source chip design manufactured at SkyWater's facility. The first major open PDK, supported by OpenLane and the IIC-OSIC-Tools flow .



- **[GlobalFoundries GF180MCU PDK](https://github.com/google/gf180mcu-pdk)**

  180nm open-source production PDK from Google and GlobalFoundries. Targets the 0.18µm 3.3/6V MCU process technology. Supported by OpenLane and other open-source flows .



- **[IHP SG13G2 Open PDK](https://github.com/IHP-GmbH/IHP-Open-PDK)**

  130nm SiGe BiCMOS open-source PDK from IHP (Leibniz Institute for High Performance Microelectronics). Targets the SG13G2 process for high-frequency and RF applications. Used in mixed-signal SoC designs including TinyWhisper .



### Design Automation & Utilities



- **[CACE](https://github.com/efabless/cace)**

  Python-based framework for running circuit simulations across PVT (process, voltage, temperature) corners. Uses YAML "datasheets" to specify test benches and corners. Runs extraction, DRC, and LVS in parallel .



- **[RALF](https://github.com/iic-jku/IIC-RALF)**

  Automatic analog layout engine. Generates layout from SPICE netlist (plus config) using Magic as layout backend without manual intervention. Early release with room for improvement in symmetry detection and device support .



- **[gdsfactory](https://github.com/gdsfactory/gdsfactory)**

  Python library for constructing layout with code. Used for RF/mm-wave component p-cell generation from Python scripts. Layout generated from ~900 lines of code for DRC-clean fabrication .



- **[Splice](https://github.com/Voidheart88/splice)**

  Fast SPICE simulator focused on better error reporting and parallel element evaluation. Supports .dc, .op, and .ac simulations with adaptive transient time-step control. Network mode for remote simulations via MessagePack protocol .



### Additional Strong Open-Source Options



- **PCB Design**: **Fritzing** (open-source, prototyping-focused), **pcb-rnd** (flexible modular editor), **tscircuit** (TypeScript/React-based PCB design), **eSim** (circuit design + simulation + PCB) .

- **Analog Simulation**: **Xyce** (parallel SPICE), **Splice** (modern SPICE with better errors), **Gnucap** (mixed-signal simulator).

- **Layout Verification**: **Netgen** (LVS), **Magic** (DRC + extraction), **KLayout** (DRC/LVS/PEX) .

- **FPGA**: **Yosys + nextpnr** (open-source FPGA flow), **SymbiFlow** (now F4PGA).



**Frameworks for building custom systems**: The **IIC-OSIC-Tools** container provides a complete, pre-configured open-source analog/mixed-signal IC design flow with Xschem, Ngspice, Magic, KLayout, and PDK support . For digital design, combine **Yosys + OpenROAD/OpenLane** with an open PDK. For PCB, **KiCad** serves as the integrated environment, with **circuitcore** adding analysis capabilities.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- EDA tools handle sensitive IP and manufacturing data; ensure proper access controls and data protection.

- **Open-source reality**: The open-source EDA ecosystem has matured to enable **complete IC design flows** — proven by silicon outcomes like TinyWhisper (4mm² mixed-signal SoC in IHP 130nm) and the 12-bit SAR ADC (SkyWater 130nm) . However, gaps remain in **large-signal noise simulation**, **accurate parasitic extraction for RF**, **scan insertion/pattern generation**, and **documentation quality** . For advanced nodes and production-critical signoff, commercial tools remain dominant.



---



**Made for IC designers, PCB engineers, hardware startups, and open-silicon advocates.**

Let's make electronic design automation more open, reproducible, and accessible.
