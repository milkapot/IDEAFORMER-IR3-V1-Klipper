It is the file modifed from originl klipper main branch in order to be able to use probe on belt printer with Y axis.
I had to modify manual_probe.py (changing Z by Y and other stuff), create probe_y.py base in probe.py. both work well for PROBE_CALIB. As MAINSAIL have a PROBE_CALIB panel now, in order to send the proper TESTY Y=value I had to modify the script directly in MAINSAIL file index.d22c661a.js as MAINSAIL is already compiled in my PI.
I tried to setup BEDMESH (only for the line on X axis against the Belt by modifing the bed_mesh.py

So far, I was able to do Calibration probe and bed mesh but the command prompt respond with erroe "bed_mesh: Invalid z-axis table length", "bed_mesh: Invalid z-axis table length
Probed table length: 3 Probed Table: "matrix value" I have difficulty to find where the Matrix is saved in order to fix it but at least I can get the probed value along the X axis on against the belt that make the bed leveling adjsutement very easy.
Of course I use capacitive probe sensor due to the Belt material but BLtouch should be ok to work with it.
Please follow instruction on Y_bed_mesh.txt to setup klipper.
