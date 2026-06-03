# FST Analysis: Investigating population differentiation levels in *An. coluzzii*

## Overview
This repository contains Python code for analyzing FST (fixation index) values for 4-fold and 0-fold sites
on chromosome 3R and X to test for population differentiation in *Anopheles coluzzii*. 

### Code
- `FST_analysis.ipynb` - Complete Jupyter notebook with all calculations and analyses

### Per-window FST calculation results
- `FST_3R_4fold_Bana_Nagare.csv` - FST values for 4-fold degenerate sites on chromosome 3R
- `FST_3R_0fold_Bana_Nagare.csv` - FST values for 0-fold degenerate sites on chromosome 3R
- `FST_X_4fold_Bana_Nagare.csv` - FST values for 4-fold degenerate sites on chromosome X
- `FST_X_0fold_Bana_Nagare.csv` - FST values for 0-fold degenerate sites on chromosome X

Descriptions of the columns on the results tables:

dfc_start: the starting DfC (Distance from Centromere) position of the non-overlapping 1Mb window
dfc_start: the end DfC position of the non-overlapping 1Mb window
orig_start: the original (counted from the telomere to centromere) position of the starting point og the non-overlapping 1Mb window
orig_end: the original position of the end point og the non-overlapping 1Mb window
fst: the mean FST value calculated over the 1Mb window
se: standard error
sites_available: the number of 4-fold or 0-fold sites found in the 1Mb window
sites_used: the number of sites that were used in the FST calculation, which excludes sites with fewer than 50 individuals contributing.
n1_eff_indiv_Bana and n2_eff_indiv_Nagare: the mean effective population size in terms of individuals in the 1Mb window that were used in the FST calculation, where n1 is for Bana village subpopulation and n2 is for Nagare subpopulation.
n_eff_seq_Bana and n_eff_seq_Nagare: the mean effective population size in terms of sequences (individuals are diploids) in the 1Mb window that were used in the FST calculation, where n1 is for Bana village subpopulation and n2 is for Nagare subpopulation.
coverage_frac_pop1 and coverage_frac_pop2: the proportion of contributing individuals out of the total available sample IDs (96 for Bana, 100 for Nagare). 
mean_ref_af_pop1 and mean_ref_af_pop2: the mean allele frequency of the reference allele over the 1Mb window for Bana and Nagare subpopulations, respectively.
mean_alt_af_pop1 and mean_alt_af_pop2: the mean allele frequency of the first alternate allele (alternate allele with the highest frequency) over the 1Mb window for Bana and Nagare subpopulations, respectively.
mean_other_af_pop1 and mean_other_af_pop2: the mean allele frequency of other alternate alleles over the 1Mb window for Bana and Nagare subpopulations, respectively.
