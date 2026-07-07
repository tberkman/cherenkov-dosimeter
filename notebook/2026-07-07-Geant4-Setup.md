## 2026-07-07

**Worked on: ** - Katz-Penfold Calculations
- Calculated the range of electron's at 2.28 MeV to be ~1.1 cm
- See working in \analysis\katz-penfold.ipynb


**Worked on: ** - Setting up a new Geant4 Simulation
- Experimented with different energies for particles
- Swapped between gamma rays and electrons
- Bug: had to fix particle name "electron" → "e-" (Geant4 uses e-)

**Worked on: ** - Geant4 electron energy sweep
- Fired electrons at 0.3, 1.0, 2.28 MeV into water geometry
- Confirmed range grows with energy; 2.28 MeV stops ~1.1 cm deep
- This matches my hand-calc (Katz-Penfold) and validates the risk assessment
