# FORUM_emissivity
Code and data for analysis in "Emissivity Retrievals with FORUM's End-to-end Simulator: Challenges and Recommendations"
https://doi.org/10.5194/amt-2021-232

## Data
The FEES outputs can be found here in an **OUTPUTS** folder:
The OUTPUTS/ folder has three sub-folders: 
- Final/ has all the full FEES retrieval run outputs used for the analysis
- SGM/ has a few synthetic scene outputs used
- transmittance_results/ has the transmittance for scene 67N 18E (not a default output of the FEES)

Each run folder contains a set of FEES ouput files, out of which two are important for the analysis:
- fe2es_l2m_out_d0001.nc - the output of the L2M retrieval module
- fe2es_sgm_ref_d0001_acq3.nc - the reference atmosphere (synthetic scene) for that case

Any additional files are only meaningful for the FORUM E2E simulator full code.

**runs.h5** is a list of all the FEES runs used (and more not uploaded) with their parameters and settings. This is a useful reference to understand the folder names.

In addition, **EMISS/** has the theoretical emissivities used in the FEES (from Huang et al. 2018)

## Code
The jupyter notebook **FORUM emissivity retrievals** has the python code for producing all the figures and tables found in the paper. It should be run in the same directory where the OUTPUTS/ folder has been extracted to.

If any questions arise feel free to email mayayami@pik-potsdam.de
