# JPLOrbitData
Orbital data for sun, planets, and some dynamical points via JPL Horizons.

This repo simply saves the text output generated from the JPL Horizons web interface.

To generate these files, do the following:

1. Go to https://ssd.jpl.nasa.gov/horizons.cgi#top

2. Choose these settings:
<code>
Ephemeris type = vector table
  
Target body = choose from list of sun + planets, satellites (for moon),
               or dynamical points (for solar system barycenter, L1, L2)
               
Coordinate origin = solar system barycenter (ssb): search for @0 in the
                    search box
                    
Time span = suggest 100 years, stepping by 1 day

Table settings:
    Type 1 (positions only)
    Leave all check boxes for uncertainties unchecked
    Output units: au & au/d
    Reference plane: ecliptic and mean equinox of reference epoch
    Reference system: ICRF/J2000.0
    Aberrations: Geometric states (no aberration; instantaneous ephemeris states)
    labels: unchecked
    delta-T: unchecked
    CSV format: checked
    object page: checked

Display output: download/save

Name files sun.txt, earth.text, etc.
</code>

