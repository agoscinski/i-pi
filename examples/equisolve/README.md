Run a simulation of the Zundel cation using a ML potential based on 
SOAP features and Gaussian processes/KRR. The potential is obtained
using https://github.com/cosmo-epfl/librascal for fitting, and a 
dedicated interface to compute energy and forces, still using librascal.
The potential can be trained using an example in the librascal source
tree, or fetched as

After having obtained the potential file, the example can be run as usual

# this does not work because model and dataset does not match, but you get the idea
pip install git+https://github.com/agoscinski/i-pi.git@equistore-potentials-draft
pip install git+https://github.com/lab-cosmo/equisolve.git@equistore-pair-potential-draft
i-pi input.xml
i-pi-py_driver -m equisolve -a water -u -o multi_spectra_script-water-potential.zip,h5o2+.extxyz