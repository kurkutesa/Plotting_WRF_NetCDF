# WRF Plot
# plotwrf.py

Python script to plot various WRF-ARW output. Written for Python 2.x

# Currently plots

- 2m temp and wind barbs
- MSLP only
- Total accumulated precipitation
- Total precipitation
- Convective precipitation
- 2m dew point temperature
- Relative humidity
- Snow accumulation
- Hail accumulation
- Simulated reflectivity
- Composite reflectivity
- LCL
- Theta-e
- Upper level charts (geopotential height, wind barbs and temperature)
- H7-H5 lapse rates
- 500mb absolute vorticity
- 0-6km Shear
- Vertical Velocity
- IR Temp
- Skew-t Plots (Uses pyMeteo package)
- Skew-t Plots using SHARPpy (Currently testing stage)
- 2-5km Updraft Helicity (Testing)

Also supports saving plots as PNG images.

Example Usage: plotwrf.py --infile filename.nc --sfc --tunit C --td --ppn --punit mm

Use plotwrf.py --help to see all possible options.

# Future improvements

- Plotting of severe weather parameters such as; CAPE, SRH, 0-6 SHR etc
- Plotting of soundings at a given latitude and longitude. Currently using pyMeteo package and SHARPpy. Need to plot more detailed soundings.
- Get data for given latitude and longitude such as max/min of variables
- Revise reflectivity routine. Possibly use FORTRAN routines to compute reflectivity

# Known Issues

- Simulated and Composite Reflectivity calculations used are for Ferrier, WSM5, fixed intercept microphysics. Plots seem to work.
- Need to fix vertical velocity calculation to use vertical motion omega equation (microbars/s) and not vertical velocity

Feel free to use and modify this script but please give credit when used. 
