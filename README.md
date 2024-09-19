# HICalculators2
Semi-experimental. Some of my Streamlit apps started failing because of Python updates, e.g. the "imp" module is replaced with "importlib". Unfortunately Streamlit didn't give this as an error message but instead complained about other, unrelated modules, even when they weren't imported... sigh. Anyway, here's what this one contains :

## Observed HI Mass
https://share.streamlit.io/rhysyt/hicalculators/main/ObservedHIMass.py
Given the total HI flux and distance to a source, this calculates the HI mass. Flux units can be mJy or Jy, distance units can be pc, kpc, or Mpc. This uses the standard formula MHI = 2.36E5d^2SHI. Optionally, it also calculates the integrated S/N of a source according to the criteria established for ALFALFA by Saintonge 2007 (https://ui.adsabs.harvard.edu/abs/2007AJ....133.2087S/abstract). This requires the line width, the velocity resolution, and rms noise level.
