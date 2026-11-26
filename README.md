# Electronics III — Analog Circuit Design in Keysight ADS

Course project covering the design, stability, frequency compensation, and noise analysis of CMOS analog amplifiers using **Keysight Advanced Design System (ADS)**.

## Project scope

1. **Two-stage CMOS operational amplifier** — transistor sizing, DC operating points, open-loop gain, frequency response, and pole identification.
2. **Frequency compensation** — shunt (dominant-pole), Miller compensation with a series nulling resistor, and common-gate compensation.
3. **System-level validation** — an op-amp symbol, slew-rate characterization, closed-loop gain, capacitive loading, and feedback compensation.
4. **Noise analysis** — a source-degenerated common-source amplifier, with parameter sweeps over resistor values, transistor geometry, bias current, temperature, and filtering.

## Selected results reported in the coursework

| Experiment | Reported result |
| --- | --- |
| Shunt compensation | 30°, 45°, and 60° phase margin at approximately 3.1 pF, 7 pF, and 21 pF |
| Miller compensation | Approximately 1 pF for 60° phase margin |
| Miller compensation with nulling resistor | Approximately 2.5 kΩ; reported bandwidth improvement from 97 MHz to 432 MHz |
| Closed-loop gain | Approximately 10 V/V (20 dB) |
| Capacitive load stability | Reported phase margins: 37.3° at 20 pF and 46.1° at 10 pF |
| External feedback compensation | Approximately 40 fF feedback capacitor for a reported 60° phase margin |

These values are **transcribed from the submitted course report**, not independently re-simulated or verified here. See the report for operating conditions and plots.

## Repository contents

- [`adsfiles/`](adsfiles/) — original ADS workspace, libraries, schematics, and data-display files.
- [`elec3_project_402101396.pdf`](elec3_project_402101396.pdf) — submitted report, including circuit images, simulation plots, and discussion (Persian).
- [`Final-Project-Electronics-3.pdf`](Final-Project-Electronics-3.pdf) — assignment specification.


## Opening the ADS project

1. Install a compatible version of **Keysight ADS**.
2. Open the workspace under `adsfiles/` using its `workspace.ads` file.
3. Inspect the library `MyLibrary_lib` and its schematics.
4. Open the corresponding `.dds` files to review available data displays. Some plots may require re-running simulations on your own machine.

**Note:** Technology libraries, transistor models, and other external dependencies may need to be configured separately for simulations to run. This repository preserves the provided project files but does not guarantee a self-contained ADS installation.

## Academic context

This work was completed as an Electronics III course project. Results are shared for educational and portfolio purposes. The repository does not claim that every reported numerical result has been independently verified.
