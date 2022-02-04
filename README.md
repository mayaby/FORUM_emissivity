# FORUM_emissivity
Code and data for analysis in "Emissivity Retrievals with FORUM's End-to-end Simulator: Challenges and Recommendations"
https://doi.org/10.5194/amt-2021-232

## Data
The FEES outputs can be found here in an **OUTPUTS** folder: **https://doi.org/10.5281/zenodo.5960223**

The OUTPUTS/ folder has three sub-folders:

- Final/ has all the full FEES retrieval run outputs used for the analysis
- SGM/ has the synthetic scene outputs shown in Figure 2
- transmittance_results/ has the transmittance for scene 67N 18E (not a default output of the FEES) shown in Figure 3

Each run folder in Final/ contains a set of FEES output files, out of which the following two are most important for the analysis:
- fe2es_l2m_out_d0001.nc - the output of the L2M retrieval module
- fe2es_sgm_ref_d0001_acq3.nc - the reference atmosphere (synthetic scene) for that case
In addition the final emissivity jacobian d_emi_num_full.dat and the atmosphere steps in the iterative retrieval process 00x_L2M_OUT.nc are also used in the analysis of the paper and are included in the folders together with additional files that are relevant for the retrieval settings.

**runs.h5** is a list of all the FEES runs used (and more not uploaded) with their parameters and settings. This is a useful reference to understand the folder names.

In addition, **EMISS/** has the theoretical emissivities used in the FEES (from Huang et al. 2018)

## Code
The jupyter notebook **FORUM emissivity retrievals** has the python code for producing all the figures and tables found in the paper. It should be run in the same directory where the OUTPUTS/ folder has been extracted to.

If any questions arise feel free to email mayayami@pik-potsdam.de
