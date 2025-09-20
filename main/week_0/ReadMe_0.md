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

# Tools Installation
********************************
## 1. Yosys 
Yosys is a framework for Verilog RTL synthesis. It currently has extensive Verilog-2005 support and provides a basic set of synthesis algorithms for various application domains. Selected features and typical applications:

   Process almost any synthesizable Verilog-2005 design
   
         - Converting Verilog to BLIF / EDIF/ BTOR / SMT-LIB / simple RTL Verilog / etc.
         - Built-in formal methods for checking properties and equivalence
         - Mapping to ASIC standard cell libraries (in Liberty File Format)
         - Mapping to Xilinx 7-Series and Lattice iCE40 and ECP5 FPGAs
         - Foundation and/or front-end for custom flows
    
### Yosys Installation Steps
    $ git clone https://github.com/YosysHQ/yosys.git
    $ cd yosys
    $ sudo apt install make # (If make is not installed please install it) 
    $ sudo apt-get install build-essential clang bison flex libreadline-dev gawk tcl-dev libffi-dev git graphviz xdot pkg-config python3 libboost-system-dev libboost-python-dev libboost-filesystem-dev zlib1g-dev
**Yosys build depends on a Git submodule called abc, which hasn't been initialized yet. You need to run the following command before running make**

    $ git submodule update --init --recursive
    $ make 
    $ sudo make install

### Verification - Yosys Installation 
![Yosys_instal](https://github.com/poonamkasturi/RTLtoGDS_RISC_V_VSD_IITGN/blob/main/main/week_0/assets/Yosys_installation.png)

### Installed Package Details
| Category | Package|Purpose |
|------|------------------|--------|
| **Compile and Buils Tools**| build-essential, clang |C/C++ compilers and build utilities |
| **Parser Tools**| bison, flex |used in HDL parsers and synthesis |
| **Shell Enhancements**| libreadline-dev, gawk |improves CLI usability and scripting |
| **Scripting Support**| tcl-dev, libffi-dev, python3 |Required for Tool Scripting and Automation|
| **Version control**| git |Essential for managing the project |
| **Visualization**| graphviz, xdot |Used for Viewing synthesis Graphs |
| **Library Managment**| pkg-config, libboost-*, zlib1g-dev |Required by many EDA tools for linking and compression |

____________________________________________________________________________________________________________

## 2. ICARUS Verilog - iverilog
Icarus Verilog is intended to compile ALL of the Verilog HDL, as described in the IEEE 1364 standard. Of course, it's not quite there yet. It also compiles a (slowly growing) subset of the SystemVerilog language, as described in the IEEE 1800 standard. For a view of the current state of Icarus Verilog, see its home page at https://steveicarus.github.io/iverilog/.

Icarus Verilog is not aimed at being a simulator in the traditional sense, but a compiler that generates code employed by back-end tools.
### iverilog Installation Steps

      $ sudo apt-get update
      $ sudo apt-get install iverilog 
   
### Verification - iverilog Installation 
![iverilog](https://github.com/poonamkasturi/RTLtoGDS_RISC_V_VSD_IITGN/blob/main/main/week_0/assets/iverilog_1.png)

________________________________________________________________________________________________________________________

## 3. GTKWave 
GTKWave is a tool to view waveforms from various file formats, such as LXT, LXT2, VZT, FST, GHW, and Verilog VCD/EVCD. 
### GTKWave Installation Steps
      $ sudo apt-get update 
      $ sudo apt install gtkwave

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
