## 2026-07-20

**Worked on:** - Geant4 Optical Physics
- Created a separate Geant4 simulation to handle Cherenkov photon simulation
- Implemented built in optical physics features to simulate the photons released in water by the Sr-90 source
    - Used G4OpticalPhysics and a water RINDEX to create Cherenkov from the band 400-550 nm
- Created a system to find the average amount of photons released per decay in a run of n decays
    - Ran at n = 200000, resulted in ~33.5 photons each time, agree with my Frank-Tamm results [analysis/photon-budget.ipynb] to 1.5%
    - Reminder: These are produced photons, not detected
