# Ex No: 02 - Design-and-Simulation-of-a-CMOS-AOI21-Complex-Gate-using-EDA-tools


## Aim
To design and simulate a CMOS inverter circuit using Synopsys EDA tools, analyze its electrical characteristics, and study its transient response

## Tools Required

### Synopsys EDA Suite
- **Synopsys Custom Compiler – For CMOS inverter schematic design.
- **Synopsys PrimeWave Design Environment – For simulation setup and waveform analysis.
- **Synopsys PrimeSim HSPICE / PrimeSim – For circuit simulation and analysis.

### Process Design Kit (PDK)
- CMOS technology library (e.g., 180nm, 45nm node)  

### Computer System
- Minimum **4GB RAM** and a **multi-core processor**
- Linux-based operating system compatible with the installed Synopsys tools.

## Procedure:
### 1. Launch Synopsys Custom Compiler Environment :
     Open Synopsys Custom Compiler and set up the working library.
     Create a new design library and associate it with the appropriate CMOS technology PDK.
     Create a new schematic cell view for the CMOS inverter design.
### 2. Schematic Design:
    Select the NMOS and PMOS transistors from the technology library.
    Connect the source terminal of the NMOS transistor to GND and its drain terminal to the output node.
    Connect the source terminal of the PMOS transistor to VDD and its drain terminal to the same output node as the NMOS transistor.
    Connect the gate terminals of both transistors together to form the input node (VIN).
    Connect the NMOS bulk terminal to GND and the PMOS bulk terminal to VDD.
    Connect a DC voltage source (VDC) to provide the supply voltage (VDD).
    Connect a pulse voltage source (VPULSE) to provide the input signal.
### 3. Simulation:
    Check the schematic for errors and verify the electrical connections.
    Create a testbench for the CMOS inverter.
    Launch Synopsys PrimeWave Design Environment.
    Select the appropriate simulator, such as PrimeSim HSPICE.
    Configure transient analysis to study the time-domain response.
    Set the simulation parameters, including supply voltage, input pulse period, rise time, fall time, and simulation stop time.
    Run the simulation and verify the simulation results.
### 4. Waveform Analysis:
    Observe the input and output voltage waveforms using the PrimeWave waveform viewer.
    Verify the inverter operation by comparing the input and output voltage levels.

## Circuit Diagram:
#### 1. CMOS Inverter:

![image](https://github.com/user-attachments/assets/e3e06487-52b2-4b56-9dcd-03c5c9394a4c)

#### 2. Schematic of CMOS Inverter:

   <img width="1033" height="733" alt="WhatsApp Image 2026-10-27 at 12 21 00 PM" src="https://github.com/user-attachments/assets/f234de9f-d81b-4759-a655-1a95ce3d015b" />


#### 3. Transient Response Setup:


<img width="936" height="475" alt="image" src="https://github.com/user-attachments/assets/145b8b37-12af-4b55-8826-11a6fc8a5227" />


## Output
#### 1.Transient Analysis and DC Response Output

<img width="1600" height="841" alt="WhatsApp Image 2026-10-27 at 12 21 10 PM" src="https://github.com/user-attachments/assets/bd160731-a49b-47fe-80b8-a598e09da0bc" />


## Results:

1.	Successfully designed the CMOS inverter schematic using Cadence EDA tools.
2.	The simulation results demonstrated the correct logic operation of the inverter, where the output voltage switches between high (Vdd) and low (0V) levels, corresponding to the input voltage transitions.










