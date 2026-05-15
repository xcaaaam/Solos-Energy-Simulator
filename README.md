# SOLOS Energy Simulator

Interactive simulation of Nikola Tesla's wireless energy transmission system based on the 1982 Marincic IEEE analysis.

![SOLOS Energy Simulator](https://img.shields.io/badge/Version-3.0-brightgreen) ![License](https://img.shields.io/badge/License-MIT-blue) ![Three.js](https://img.shields.io/badge/Three.js-r128-orange)

## 🌍 Live Demo

Open `solos_energy_simulator.html` in any modern browser (Chrome, Firefox, Safari, Edge).

## ✨ Features

- **Real-time 3D Globe** with Three.js visualization
- **Interactive Node System** - Add, configure, and visualize transmission nodes worldwide
- **Accurate ELF Physics** - Based on Marincic's 1982 analysis of Tesla's system
- **Material Comparison** - Test different conductors (Earth, graphene, superconductors, etc.)
- **Critical System Monitoring** - Real-time alarms when system parameters become unstable
- **Horizontal JARVIS-style UI** - Clean panel layout inspired by sci-fi interfaces
- **Educational Glossary** - Explanations of key concepts in simple language

## 🎯 What This Simulates

Nikola Tesla's ambitious plan to transmit electrical energy wirelessly around the globe using:
- **Extremely Low Frequency (ELF)** waves (6-10 Hz)
- **Earth resonance** - The planet acting as a resonant cavity
- **Standing waves** - Energy accumulating at specific points (antinodes)
- **Ionospheric return path** - Using the upper atmosphere as a conductor

## 🔬 Scientific Basis

Based on:
- **A.S. Marincic (1982)** "Nikola Tesla and the Wireless Transmission of Energy", IEEE Transactions on Power Apparatus and Systems
- **Tesla's Patents** (1897-1905): US645576, US787412, and laboratory notes from Colorado Springs (1899)
- **Modern ELF Research** - Schumann resonance, ionospheric propagation, submarine communications

## 🚀 Quick Start

1. Download `solos_energy_simulator.html`
2. Open in browser (no server required - standalone file)
3. Adjust parameters with sliders
4. Add transmission nodes around the globe
5. Watch the real-time efficiency calculations

## 🎮 Controls

### Global Parameters
- **Frequency** (1-100 Hz): ELF transmission frequency. Tesla used 6 Hz.
- **Voltage** (1-200 MV): Transmitter voltage. Higher = more ionization.
- **Atmospheric Conductivity** (0-1): Ionosphere conductivity factor.
- **Target Distance** (1-40 Mm): Transmission range. Earth circumference = 40 Mm.

### Globe View
- **Drag to rotate** the globe
- **Click nodes** to select and edit
- **Toggle layers**: Waves, Atmosphere, Connections, Tesla Labs, Standing Waves

### System Alarms

The simulator monitors system health and triggers alarms when:
- ⚠️ **Efficiency < 0.0001%**: System collapse - transmission impossible
- ⚠️ **Antenna efficiency < 0.001%**: Antenna failure at current frequency
- ⚠️ **Voltage > 180 MV**: Atmospheric ionization threshold
- ⚠️ **Out of resonance**: Frequency outside Tesla's 5-9 Hz optimal range

When alarms trigger, press **RESTART** to reset to safe parameters.

## 📊 Why Tesla's Vision Failed

The simulator demonstrates the core problem:

| Parameter | Tesla 1905 | Modern Analysis |
|-----------|-----------|-----------------|
| **Earth Resonance** | ✅ Correctly predicted ~6-8 Hz | ✅ Confirmed (Schumann resonance 7.83 Hz) |
| **Standing Waves** | ✅ Predicted global patterns | ✅ Confirmed in ELF propagation |
| **Low Attenuation** | ✅ ELF has minimal loss | ✅ 0.25-1.0 dB/Mm at 10-100 Hz |
| **Antenna Efficiency** | ❌ Assumed high efficiency | ❌ **Only 0.026% at 45 Hz** |

**Conclusion**: Even with perfect conductors (graphene, superconductors), ELF antenna efficiency is so low (~0.001-0.1%) that global wireless power remains impractical.

## 🧪 Experiment Ideas

Try these configurations:

### 1. **Tesla's Original Setup**
- Frequency: 6 Hz
- Voltage: 10 MV
- Material: Dry Earth
- Node: Wardenclyffe (40°N, 74°W)
- **Result**: 0.0014% efficiency

### 2. **Modern Graphene Network**
- Frequency: 8 Hz (Schumann)
- Voltage: 50 MV
- Material: Graphene
- Nodes: 4 globally distributed
- **Result**: ~0.02% efficiency (14x improvement, still impractical)

### 3. **Theoretical Superconductor Grid**
- Frequency: 6 Hz
- Voltage: 100 MV
- Material: Superconductor HTS
- Nodes: 8 nodes at antipode pairs
- **Result**: ~0.05% efficiency (best case, still far too low)

### 4. **Trigger System Collapse**
- Frequency: 80 Hz
- Voltage: 5 MV
- Distance: 35 Mm
- **Result**: CRITICAL ALARM - System efficiency < 0.00001%

## 📖 Glossary

The simulator includes an interactive glossary explaining:
- **Attenuation** - Energy loss over distance
- **ELF Frequency** - Why ultra-low frequencies matter
- **Earth Resonance** - Tesla's 6 Hz calculation
- **Conductivity** - Material comparison (copper vs Earth vs graphene)
- **Standing Waves** - Energy amplification at antinodes
- **Ionosphere** - Upper atmosphere as return conductor
- And more...

## 🛠️ Technical Stack

- **Three.js r128** - 3D globe rendering
- **Vanilla JavaScript** - No framework dependencies
- **CSS Grid** - Responsive horizontal layout
- **HTML5 Canvas** - Secondary visualizations
- **Pure CSS** - Custom green/yellow theme (no emoticons)

## 📝 File Structure

```
solos_energy_simulator.html    # Standalone HTML file (all-in-one)
README.md                       # This file
LICENSE                         # MIT License
```

## 🎨 Design Philosophy

- **No emoticons** - Professional scientific interface
- **Horizontal layout** - JARVIS/control panel aesthetic
- **Light text hierarchy** - Important text bright yellow (#F0FE26), secondary text light yellow (#F7FF80)
- **Real-time feedback** - Parameters update immediately
- **Critical alarms** - Visual + text warnings for system failures

## 🤝 Contributing

This is an educational tool. Contributions welcome:
- Improved physics models
- Additional materials database
- Historical Tesla quotes/references
- UI improvements
- Bug fixes

## 📚 References

1. **Marincic, A.S.** (1982). "Nikola Tesla and the Wireless Transmission of Energy." *IEEE Transactions on Power Apparatus and Systems*, Vol. PAS-101, No. 10, pp. 4064-4068.

2. **Tesla, N.** (1900). US Patent 645,576 "System of Transmission of Electrical Energy"

3. **Tesla, N.** (1905). US Patent 787,412 "Art of Transmitting Electrical Energy Through the Natural Mediums"

4. **Burrows, M.L.** (1978). *ELF Communications Antennas.* Peter Peregrinus.

5. **Wait, J.R.** (1974). "Historical background and introduction to extremely low frequency (ELF) propagation." *IEEE Transactions on Communications*, COM-22.

6. **Tesla, N.** (1899-1900). *Colorado Springs Notes.* Belgrade: Nikola Tesla Museum, 1976.

## ⚖️ License

MIT License - See LICENSE file

## 🙏 Acknowledgments

- Nikola Tesla for his visionary (if impractical) wireless power concept
- A.S. Marincic for rigorous IEEE analysis
- Three.js community for 3D rendering framework

---

**Educational Use Only** - This simulator is for understanding why Tesla's global wireless power system was physically impossible with any known technology. It does not encourage attempts to build such systems.

Built with ⚡ for education and Tesla appreciation.
