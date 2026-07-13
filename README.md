# cherenkov-dosimeter

This project is an open-source low cost method to detect and quantify the Cherenkov light produced by radioactive beta particle sources (specifically Sr-90/Y-90, 0.1 uci, the legal limit for posession). Because this source is ~1000x weaker, if not more, than what clinical systems that actually use this technique use, the signal is microscopic. In order to actually reaed that signal, the project uses techniques borrowed from astrophotography (a cooled camera, long exposures, frame-stacking, etc) to pull the signal out from beneath the noisy floor. Furthermore, narrowband filters are used to separate the known spectral shape Cherenkov light produces from the background, and the result is calibrated to a radiation dose map and validated against custom built Geant4 monte-carlo sims. The entire system is intended to be accessible, for the purpose of research and education. (open-source and <$3000, as clinical devices cost upwards of 100000)

Main contributions of this project to the field:
1. Spectral discrimination at exempt activity. Spectral separation of Cherenkov from
background is established in clinical/preclinical imaging. A contribution from this project for the field is demonstrating it in the photon-starved exempt-activity regime, grounded in the Frank-Tamm formula prediction

2. Geometry-dependent dose-conversion characterization. The light-to-dose conversion's
dependence on geometry is acknowledged in clinical literature but not systematically
characterized at exempt activity. This project measures it across multiple geometries,
cross-validated against Geant4, as a relative dataset (which sidesteps the ±20%
absolute-activity uncertainty).