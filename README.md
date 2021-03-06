# Analyze the data by force-induced remnant magnetization spectroscopy (FIRMS)

A. Signal Analysis

The code, force_analysis_gui_tk.py, is used to analyze the magnetic signal in measurements. In the beginning, it converts the unit of signal from the nano-ampere (nA) to pico-tesla (pT) by comparing with the reference signal from a function generator, which provides a stable 150 pT as the input signal through a Helmholtz coil. Then, all measurements are subtracted from the background signal to get the change of magnetic field. Finally, the measurement is corrected from the fluctuation of laser to get a clear signal. It can be seem as the magnetic field generated by a magnetic dipole moment to get the amount of magnetic particles with the specific interaction with the sample system.

The code, function_MRI.py, contains the functions used in force_analysis_gui_tk.py.

B. File Splitter

The code, file_preparation_new.py, splits the measurement output from LabVIEW into files with individual experimental condition (i.e. lasting time, voltage, and frequency) when the piezoelectric material is the source of acoustic radiation force.
