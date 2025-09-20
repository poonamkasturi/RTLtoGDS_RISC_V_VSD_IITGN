# 🛠️ Week_0 : Foundational Week : 
## Open-Source EDA Toolchain Setup on Ubuntu

Welcome to my visual walkthrough of installing and configuring essential open-source tools for ASIC design and simulation.
This week focused on setting up the development environment and installing the essential open-source tools
This repository documents the setup process for tools like Yosys, Icarus Verilog, GTKWave, NGSpice, Magic VLSI, Docker, and Python
All running on Ubuntu inside a VirtualBox VM.
________________________________________

The goal was to create a reliable and efficient workspace for synthesis, simulation, and design tasks.

## INSTALLATION ENVIRONMENT

Oracle virtual machine link https://www.virtualbox.org/wiki/Downloads

### VIRTUAL MACHINE CONFIGURATION SET-UP

| Specification | Details|
|---------------|----------------|
| **Operating System**| Ubuntu 20.04+ |
| **RAM**| 6GB |
| **Storage**| 50 GB HDD |
| **vCPU**| 4|

![VM_set_up](https://github.com/poonamkasturi/RTLtoGDS_RISC_V_VSD_IITGN/blob/main/main/week_0/assets/VM%20set_up.png)


## System Check for TOOL INSTALLATION and Verification

## 📂 Contents

| Tool | Description|Folder |
|------|------------------|--------|
| **Yosys**| RTL synthesis for Verilog designs | yosys/ |
| **iverilog**| Verilog Simulation and Compilation | icarus-verilog/ |
| **GTKwave**| Waveform Viewer & Analysis | gtkwave/ |
| **Ngspice**| Circuit-level simulation | ngspice/ |
| **Magic VLSI**| Layout Design & DRC Verification | magic-vlsi/ |
| **Docker**| Containerized environment setup | docker/ |
| **Python & pip**| Virtual environments and scripting tools | python-env/ |

------------------------------------------------------------------------------------

## Day 0 - Tools Installation
## Yosys

$ git clone https://github.com/YosysHQ/yosys.git
$ cd yosys 
$ sudo apt install make # (If make is not installed please install it) 
$ sudo apt-get install build-essential clang bison flex \
    libreadline-dev gawk tcl-dev libffi-dev git \
    graphviz xdot pkg-config python3 libboost-system-dev \
    libboost-python-dev libboost-filesystem-dev zlib1g-dev
$ make 
$ sudo make install

### Verification - Yosys Installation 
![Yosys_instal](https://github.com/poonamkasturi/RTLtoGDS_RISC_V_VSD_IITGN/blob/main/main/week_0/assets/Yosys_installation.png)


### Verification - iverilog Installation 
![iverilog](https://github.com/poonamkasturi/RTLtoGDS_RISC_V_VSD_IITGN/blob/main/main/week_0/assets/iverilog_1.png)

### Verification - GTKWave Installation 
![GTKWave](https://github.com/poonamkasturi/RTLtoGDS_RISC_V_VSD_IITGN/blob/main/main/week_0/assets/GTKWave.png)

### Verification - Ngspice Installation 
![Ngspice](https://github.com/poonamkasturi/RTLtoGDS_RISC_V_VSD_IITGN/blob/main/main/week_0/assets/ngspice.png)

### Verification - Magic VLSI Installation 
![Magic](https://github.com/poonamkasturi/RTLtoGDS_RISC_V_VSD_IITGN/blob/main/main/week_0/assets/magic.png)

### Verification - Docker Installation 
![Docker](https://github.com/poonamkasturi/RTLtoGDS_RISC_V_VSD_IITGN/blob/main/main/week_0/assets/Docker.png)

### Versions of the tools installed
![Versions_Tools](https://github.com/poonamkasturi/RTLtoGDS_RISC_V_VSD_IITGN/blob/main/main/week_0/assets/versions.png)
