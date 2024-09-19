# HICalculators2
Semi-experimental. Some of my Streamlit apps started failing because of Python updates, e.g. the "imp" module is replaced with "importlib". Unfortunately Streamlit didn't give this as an error message but instead complained about other, unrelated modules, even when they weren't imported... sigh. Anyway, here's what this one contains :

## Observed HI Mass
Available through Streamlit at : https://share.streamlit.io/rhysyt/hicalculators/main/ObservedHIMass.py<br>
Given the total HI flux and distance to a source, this calculates the HI mass. Flux units can be mJy or Jy, distance units can be pc, kpc, or Mpc. This uses the standard formula MHI = 2.36E5d^2SHI. Optionally, it also calculates the integrated S/N of a source according to the criteria established for ALFALFA by Saintonge 2007 (https://ui.adsabs.harvard.edu/abs/2007AJ....133.2087S/abstract). This requires the line width, the velocity resolution, and rms noise level.

## Column Density Calculator
Available through Streamlit at : [https://share.streamlit.io/rhysyt/hicalculators/main/ColumnDensityCal.py](https://columndensitycalpy.streamlit.app/)<br>
Given the mass and size of an object (in different units), this calculates the average column density of the material. Returns the result in both atoms cm^-2 and Msolar pc^-2. Although labelled as HI, this will work equally well for anything else. Note HI tends to saturate at ~10 Msolar pc^2 and is rarely found at levels at or below 10^17 cm^-2 (the tendency of to routinely use different units for the same measurement in different contexts is one very good reason such a calculator is needed !).

## Travel Time
Available through Streamlit at [https://share.streamlit.io/rhysyt/hicalculators/main/TravelTime.py](https://traveltimepy.streamlit.app/)<br>
Another useful way to conver between different units. Does simple, linear calculations of either : 1) time taken to travel a given distance at a given speed; 2) the distance travelled in a given time at a given speed; 3) the average speed to travel a given distance in a given time. Very simple, but since we generally use km/s for speed but kpc for distances, the unit conversion is handy to have.
