# FORUM_emissivity
Code and data for analysis in https://doi.org/10.5194/amt-2021-232

## Data
The FEES outputs can be found here in an OUTPUTS folder:
The OUTPUTS/ folder has three sub-folders: 
- Final/ has all the full FEES retrieval run outputs used for the analysis
- SGM/ has a few scene outputs for Figure 2
- transmittance_results/ has the transmittance for scene 6718 which is not a default output of the FEES

EMISS/ has the theoretical emissivities used in the FEES (from Huang et al. 2018)

runs.h5 is a dataset with all the runs used (and more not uploaded) with their parameters and settings. This is a useful reference to understand the folder names.

Each folder contains a set of netCDF files for the cases treated in the paper. Each directory contains three files:
- fe2es_fei_out_d0001.nc - the output of the FEI imager
- fe2es_fsi_out_d0001.nc - the output of the FSI spectrometer
- fe2es_sgm_ref_d0001_acq3.nc - The reference atmosphere for that case

Any additional files are only meaningful for the FORUM E2E simulator full code.

## Code
The jupyter notebook has the code for producing all the figures and tables found in the paper. It can be run in the same directory where the OUTPUTS/ and other folders can be found

If any questions arise feel free to email mayayami@pik-potsdam.de
