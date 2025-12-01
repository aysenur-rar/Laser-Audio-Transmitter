# Free-Space Optical (FSO) Audio Transceiver

### Project Overview
This project demonstrates a wireless optical communication system capable of transmitting high-fidelity analog audio signals over a distance of 10+ meters using a collimated laser beam. The system integrates a custom-designed optical lens assembly (simulated in Ansys Zemax) with a Class-A analog modulation circuit (designed in KiCad).


### 🚀 Key Features
* **Optical Range:** >10 meters with <2 mrad beam divergence.
* **Modulation Scheme:** Analog Intensity Modulation (IM/DD).
* **Optical Power:** <5mW (Class 3R Safety Compliance).
* **Bandwidth:** 20Hz - 20kHz (Full Audio Spectrum).

### 🛠 Technical Implementation

#### 1. Electronics Design (KiCad)
* **Topology:** Common Emitter Voltage Amplifier with DC Bias network.
* **Bias Point Analysis:** Designed a stable Q-point ($V_{bias} \approx 1.6V$) to maintain the laser diode in its linear region, preventing clipping of the AC audio signal.
* **Current Limiting:** Integrated a calculated emitter degeneration resistor ($33\Omega$) to cap forward current at safe limits (~200mA) while maintaining gain.

#### 2. Optical Design (Ansys Zemax)
* **Objective:** Collimation of a diverging laser diode source to maximize power transfer.
* **Methodology:** Performed RMS Spot Radius optimization on a plano-convex lens system.
* **Result:** Achieved a highly collimated beam with minimal wavefront error.
