# Ex No: 02 - Design-and-Simulation-of-a-CMOS-AOI21-Complex-Gate-using-EDA-tools


## Aim
To design and simulate Y=(A+BC)' circuit using Synopsys EDA tools, analyze its electrical characteristics, and study its transient response

## Tools Required

### Synopsys EDA Suite
- Synopsys Custom Compiler – For CMOS inverter schematic design.
- Synopsys PrimeWave Design Environment – For simulation setup and waveform analysis.
- Synopsys PrimeSim HSPICE / PrimeSim – For circuit simulation and analysis.

### Process Design Kit (PDK)
- CMOS technology library (e.g., 180nm, 45nm node)  

### Computer System
- Minimum **4GB RAM** and a **multi-core processor**
- Linux-based operating system compatible with the installed Synopsys tools.

## Procedure:
### 1. Launch Synopsys Custom Compiler Environment :
     Open Synopsys Custom Compiler and set up the working library.
     Create a new design library and associate it with the appropriate CMOS technology PDK.
     Create a new schematic cell view for the CMOS design.
### 2. Schematic Design:
     Select three NMOS transistors and three PMOS transistors from the technology library.
     Construct the NMOS pull-down network (PDN) by connecting transistor N1 in parallel with the series combination of transistors N2 and N3.
     Connect the gate terminal of N1 to input A, the gate terminal of N2 to input B, and the gate terminal of N3 to input C.
     Connect the drain terminal of N1 and the drain terminal of N2 to the output node Y.
     Connect the source terminal of N1 to GND and the source terminal of N3 to GND. Connect the source terminal of N2 to the drain terminal of N3.
     Construct the PMOS pull-up network (PUN) as the complementary connection of the NMOS pull-down network.
     Connect PMOS transistor P1 in series with the parallel combination of PMOS transistors P2 and P3.
     Connect the gate terminal of P1 to input A, the gate terminal of P2 to input B, and the gate terminal of P3 to input C.
     Connect the source terminal of P1 to VDD. Connect the drain terminal of P1 to the common source terminals of P2 and P3.
     Connect the drain terminals of P2 and P3 to the output node Y, which is common to the NMOS pull-down network.
     Connect the bulk terminals of all PMOS transistors to VDD and the bulk terminals of all NMOS transistors to GND.
     Connect a DC voltage source (VDC) to provide the required supply voltage (VDD).
     Connect three pulse voltage sources (VPULSE) to provide the input signals A, B and C with appropriate pulse widths and time periods.
     Connect the ground terminals of the voltage sources to the common ground node.
     Save the schematic and perform Check and Save to verify the circuit connectivity.
     Create a testbench and perform transient analysis to verify the output response for all possible input combinations.
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
#### 1. CMOS Logic: Y=(A+BC)'

<img width="190" height="261" alt="image" src="https://github.com/user-attachments/assets/4eeded35-4724-4994-9108-430d4669a791" />

#### 2. Schematic of CMOS L0gic:

   <img width="1033" height="733" alt="WhatsApp Image 2026-10-27 at 12 21 00 PM" src="https://github.com/user-attachments/assets/f234de9f-d81b-4759-a655-1a95ce3d015b" />


#### 3. Transient Response Setup:


<img width="936" height="475" alt="image" src="https://github.com/user-attachments/assets/145b8b37-12af-4b55-8826-11a6fc8a5227" />


## Output
#### 1.Transient Analysis

<img width="1600" height="841" alt="WhatsApp Image 2026-10-27 at 12 21 10 PM" src="https://github.com/user-attachments/assets/bd160731-a49b-47fe-80b8-a598e09da0bc" />


## Results:

1.	Successfully designed the CMOS logic schematic using Synopsys EDA tools.
2.	The circuit functionality was verified using transient analysis by applying different combinations of input signals A, B and C. The simulated output response was found to match the expected truth table.










