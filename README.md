# vasp_wavecar_parity

# Wang Dinghui
# DZ1722031@smail.nju.edu.cn
# Nanjing University

# compile the code by:
"""
ifort -o parity.x wavetrans.f90 parity.f90 main.f90 -assume byterecl
"""

# WAVETRANS.F90 code modified from
# https://www.andrew.cmu.edu/user/feenstra/wavetrans/
# by
# R. M. Feenstra and M. Widom
# Department of Physics, Carnegie Mellon University, Pittsburgh, PA 15213

# Please make sure the following points:
- Setting LWAVE=.TRUE. in your INCAR and remain WAVECAR.
- Your system DOES have Inversion Symmetry.
- Exact Inverstion Symmetry Coordinate corresponding to POSCAR.
- You know what's you are doing.

# Now this code is not tested in magnetic system yet!
