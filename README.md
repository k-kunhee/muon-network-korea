# Muon Network Korea

**A student-led open-data muon detector network in South Korea**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Data License: CC BY 4.0](https://img.shields.io/badge/Data%20License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)
[![Status: Active](https://img.shields.io/badge/Status-Active-brightgreen.svg)]()
[![Detector: CosmicWatch v3X](https://img.shields.io/badge/Detector-CosmicWatch%20v3X-blue.svg)](https://github.com/spenceraxani/CosmicWatch-Desktop-Muon-Detector-v3X)

---

## Overview

This repository documents the design, deployment, and scientific output of a muon detector network being developed across South Korea. The project is based on the [CosmicWatch v3X](https://github.com/spenceraxani/CosmicWatch-Desktop-Muon-Detector-v3X) desktop muon detector, developed originally at MIT and the Polish National Centre for Nuclear Research (NCBJ), and currently led by the University of Delaware.

South Korea occupies a scientifically significant and underutilized position in global cosmic ray research. The Korean Peninsula spans a vertical geomagnetic cutoff rigidity gradient of approximately **10–12 GV** (from the DMZ at ~38°N to Jeju Island at ~33°N) — a range where systematic ground-level monitoring networks are nearly absent. Combined with Gangwon-do's exceptional altitude gradient (sea level to 1,708 m within ~60 km), proximity to two world-class underground laboratories ([Yemilab](https://yemilab.ibs.re.kr) and [Y2L](https://y2l.ibs.re.kr)), and the operational [Gamaksan Neutron Monitor](https://nmdb.eu), this network is positioned to produce measurements that are genuinely novel in the global context.

All collected data will be made publicly available under the CC BY 4.0 license.

---

## Scientific Goals

### Primary
- **Altitude survey**: Systematic measurement of muon flux across the Gangwon-do elevation transect (sea level → Daegwallyeong Pass, 850 m → Seoraksan, 1,708 m), compared against EXPACS/PARMA theoretical predictions
- **Barometric coefficient measurement**: Determination of the muon rate–pressure correlation coefficient for South Korea, to be compared with published values (Kim et al. 2012: −0.1191 ± 0.0054 %/hPa at Hanyang University)
- **Long-term cosmic ray monitoring**: Continuous muon rate logging for space weather events including Forbush decreases, with cross-correlation against NMDB neutron monitor data

### Secondary
- Muon Snow Water Equivalent (μ-SWE) measurement in Gangwon-do mountain snowpack
- Muon absorption measurement in Gangwon-do limestone cave (Hwanseongul, Samcheok)
- Multi-station coincidence array for Extensive Air Shower (EAS) detection

### Long-term
- Establishment of a multi-school network spanning South Korea's latitude–altitude range
- Contribution to the [CREDO](https://credo.science) (Cosmic Ray Extremely Distributed Observatory) international collaboration

---

## Detector

| Parameter | Value |
|-----------|-------|
| Platform | CosmicWatch v3X |
| Scintillator | 5 × 5 × 1 cm BC-408 plastic scintillator |
| Photodetector | Silicon Photomultiplier (SiPM) |
| Microcontroller | Raspberry Pi Pico (RP2040) |
| Environmental sensor | BMP280 (temperature, pressure) |
| Data storage | MicroSD card |
| External trigger | BNC coincidence port |
| Approximate unit cost | ~$100 USD |

The v3X detector is described in detail in: Axani et al. (2025), *arXiv:2508.12111*.

---

## Repository Structure

```
muon-network-korea/
│
├── data/                    # Raw and corrected measurement data (CSV)
│   ├── altitude-survey/
│   ├── barometric/
│   └── long-term/
│
├── analysis/                # Python analysis scripts and Jupyter notebooks
│   ├── pressure_correction.ipynb
│   ├── altitude_survey.ipynb
│   └── utils.py
│
├── docs/                    # Technical documentation
│   ├── detector-build/
│   ├── ko/                  # Korean-language documentation (한국어)
│   └── station-log/
│
├── hardware/                # 3D-printable accessories, enclosure designs
│
└── README.md
```

> **Note**: Data and analysis directories will be populated as measurements are collected. Current status: detector procurement phase.

---

## Current Status

| Milestone | Status |
|-----------|--------|
| Repository setup | ✅ Complete |
| Detector parts ordered | ✅ Complete |
| Python analysis environment | 🔧 In progress |
| EXPACS theoretical predictions | 🔧 In progress |
| Detector assembly | ⏳ Pending (May 2026) |
| Barometric coefficient measurement | ⏳ Pending |
| Altitude survey | ⏳ Pending |
| First data release | ⏳ Pending |

---

## Data Policy

All measurement data produced by this project are released publicly under the **Creative Commons Attribution 4.0 International (CC BY 4.0)** license.

Users are free to share and adapt the data for any purpose, provided appropriate credit is given. See `DATA_LICENSE` for details.

Analysis code and software are released under the **MIT License**.

---

## Related Projects and Collaborations

- [CosmicWatch v3X](https://github.com/spenceraxani/CosmicWatch-Desktop-Muon-Detector-v3X) — University of Delaware
- [CREDO](https://credo.science) — Cosmic Ray Extremely Distributed Observatory
- [NMDB](https://nmdb.eu) — Neutron Monitor Database
- [HiSPARC](https://hisparc.utah.edu) — High School Project on Astrophysics Research with Cosmics
- [QuarkNet](https://quarknet.org) — Fermilab / Notre Dame

---

## References

- Axani, S. N. et al. (2025). *CosmicWatch: The Desktop Muon Detector (v3X)*. arXiv:2508.12111
- Jung, G. et al. (2025). *Gamaksan Neutron Monitor*. J. Astron. Space Sci.
- Kim, J. et al. (2012). *Barometric coefficient measurement at Hanyang University*. J. Korean Phys. Soc.
- Gugerli, R. et al. (2022). *Muon snow water equivalent measurements*. The Cryosphere.

---

## Contact

**Project lead**: [Kunhee Kim] | [Korean Minjok Leadership Academy], Gangwon-do, South Korea
**GitHub**: [@k-kunhee](https://github.com/k-kunhee)
**Email**: [kunhee.kim09@gmail.com]

Inquiries regarding data access, collaboration, or network participation are welcome.

---

## Acknowledgements

The CosmicWatch v3X detector platform was developed by Prof. Spencer N. Axani and colleagues at the University of Delaware.

---

*Last updated: March 2026*
