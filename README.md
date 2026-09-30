# Analog Integrated Electronics

This repository contains laboratory reports and simulation work completed for the **Analog Integrated Electronics Laboratory (EEE 4878)** using Cadence Virtuoso and related IC design and verification tools.

## Experiments

| No. | Experiment                                                           | Main Topics                                                                                                                                                             |
| --- | -------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 01  | **MOS Transistor Characteristics and Parameter Analysis**            | I<sub>D</sub>–V<sub>GS</sub>, I<sub>D</sub>–V<sub>DS</sub>, threshold voltage, transconductance, output resistance, and figure of merit                                 |
| 02  | **Single-Stage Common-Source CMOS Amplifier**                        | Common-source amplifier, load configurations, voltage gain, output swing, frequency response, and transistor sizing                                                     |
| 03  | **Bandgap Voltage Reference Circuit**                                | Bandgap reference design, V<sub>BE</sub> and ΔV<sub>BE</sub>, temperature compensation, temperature coefficient, supply-voltage variation, and 1 V reference generation |
| 04  | **Two-Stage CMOS Operational Amplifier – DC and AC Characteristics** | Two-stage op-amp, DC transfer characteristics, offset voltage, frequency response, gain, GBW, phase margin, PSRR, and CMRR                                              |
| 05  | **Layout Design and Verification of CMOS**                           | CMOS inverter layout, transistor sizing, multi-finger structures, body ties, routing, DRC, and LVS verification                                                         |

---

## 01 — MOS Transistor Characteristics and Parameter Analysis

Study of the basic current–voltage characteristics and key parameters of MOS transistors using Cadence Virtuoso.

### Topics Covered

* I<sub>D</sub>–V<sub>GS</sub> characteristics
* I<sub>D</sub>–V<sub>DS</sub> characteristics
* Threshold voltage (V<sub>TH</sub>)
* Transconductance (g<sub>m</sub>)
* Output resistance (r<sub>o</sub>)
* Figure of merit (g<sub>m</sub>/I<sub>D</sub>)
* NMOS and PMOS characteristics
* Mobility comparison

---

## 02 — Single-Stage Common-Source CMOS Amplifier

Design, layout, simulation, and verification of a single-stage common-source CMOS amplifier using Cadence Virtuoso.

### Load Configurations

* Diode-connected load
* Current-source load
* Triode-region load

### Analysis

* Voltage gain
* Output swing
* Frequency response
* Power consumption
* Effect of transistor sizing
* Effect of load configuration

---

## 03 — Bandgap Voltage Reference Circuit

Design and characterization of a CMOS-based bandgap voltage reference circuit using Cadence Virtuoso and the GPDK090 technology library.

### Topics Covered

* Bandgap reference voltage generation
* V<sub>BE</sub> and ΔV<sub>BE</sub> temperature characteristics
* Temperature compensation
* DC simulation of V<sub>REF</sub>
* Temperature sweep analysis
* Temperature coefficient calculation
* Supply-voltage variation
* Zero-temperature-coefficient condition
* Design of a 1 V bandgap reference generator

### Simulation Highlights

* V<sub>REF</sub> ≈ 0.8136 V at V<sub>DD</sub> = 3.3 V
* Temperature sweep: 10°C–50°C
* Temperature coefficient at 27°C: −1.2066 mV/°C
* Supply-voltage sweep: 3.1 V–3.5 V
* 1 V bandgap reference design
* Temperature coefficient of the 1 V reference: −644.337 ppm/°C

---

## 04 — Two-Stage CMOS Operational Amplifier – DC and AC Characteristics

Design and simulation of a two-stage CMOS operational amplifier using Cadence Virtuoso.

### Topics Covered

* NMOS differential input stage
* PMOS active load
* Common-source second stage
* Frequency compensation
* DC transfer characteristics
* Input offset voltage
* AC frequency response
* Voltage gain
* Gain bandwidth
* Phase margin
* Gain margin
* Power-supply rejection ratio (PSRR)
* Common-mode rejection ratio (CMRR)
* Output offset correction through transistor sizing

---

## 05 — Layout Design and Verification of CMOS

Design and physical verification of a CMOS inverter using **Cadence Virtuoso Layout Suite XL** and a **45 nm CMOS process design kit**.

The experiment demonstrates the transition from a transistor-level schematic to a physical IC layout, including device placement, multi-finger transistor implementation, routing, body-tie connections, and physical verification.

### Topics Covered

* CMOS inverter design
* PMOS and NMOS transistor sizing
* Schematic-driven layout generation
* Physical transistor placement
* Multi-finger transistor structures
* Body-tie implementation
* Signal and supply routing
* Design Rule Checking (DRC)
* Layout Versus Schematic (LVS)
* Physical layout verification

### Transistor Dimensions

* PMOS: W = 960 nm, L = 45 nm
* NMOS: W = 480 nm, L = 45 nm

The PMOS width was selected to be twice the NMOS width to account for the difference in carrier mobility and provide more balanced switching characteristics.

### Verification

* **DRC:** Used to check the layout against physical design rules and fabrication-related geometric constraints.
* **LVS:** Used to compare the extracted layout netlist with the original schematic and verify circuit connectivity.
* **Result:** The final layout achieved a clean DRC result and a successful LVS comparison.

### Tools Used

* Cadence Virtuoso Schematic Editor
* Cadence Virtuoso Layout Suite XL
* 45 nm CMOS PDK
* Pegasus DRC
* Pegasus LVS
* Quantus Parasitic Extraction

---

## Tools & Technologies

* **Cadence Virtuoso**
* **Cadence Virtuoso Layout Suite XL**
* **Spectre Simulator**
* **GPDK090 Technology Library**
* **45 nm CMOS PDK**
* **Cadence ADE**
* **Virtuoso Calculator**
* **Pegasus DRC**
* **Pegasus LVS**



---

## Course

**EEE 4878 — Analog Integrated Electronics Laboratory**
**Islamic University of Technology (IUT)**

## Repository Structure

```text
analog-integrated-electronics/
│
├── README.md
│
├── 01 - MOS Transistor Characteristics and Parameter Analysis.pdf
├── 02 - Single-Stage Common-Source CMOS Amplifier.pdf
├── 03 - Bandgap Voltage Reference Circuit.pdf
├── 04 - Two-Stage CMOS Operational Amplifier - DC and AC Characteristics.pdf
└── 05 - Layout Design and Verification of CMOS.pdf
```
