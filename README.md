# GVP_2023:

This repository contains all the scripts necessary to reproduce figures in "Stochastic Systems Biology of the Cell Using Single-cell Genomics Data." All figure components are output in `figs/` in `pdf` and `png` (450 DPI) formats. Font sizes vary.

* Figure 1
  * Panel d: run `gg230227_cartoons.ipynb`. This will generate the files `fig1d_txmodels` (transcription models) and `fig1d_reactors` (reactor models).
* Figure 2
  * Panel a: run the first cell and the last two cells of `gg230117_emptydrops.ipynb`. This will generate the file `fig2a_poissprod`. 
  * Panels b, c, d, e: download the raw data from [Zenodo](https://zenodo.org/record/7694182). Note this link is not yet active. I can activate it if necessary. Run `gg230117_emptydrops.ipynb`. This will generate the files `fig2bcde`, which has the content for the body, and `emptydrops_supp_pbmc_1k_v3`, which has the content for the supplement.
  * Supplements: run the five other `emptydrops` notebooks. They will generate `emptydrops_supp_brain_nuc_5k_v3`, `emptydrops_supp_desai_dmso`, `emptydrops_supp_heart_1k_v3`, `emptydrops_supp_neuron_1k_v3`, and `emptydrops_supp_pbmc_1k_v2`. 
    * Note: each notebook can take up to 15 minutes to run (gene-gene correlations are slow to calculate and store).
* Figure 3
  * Panel a: run `gg230227_cartoons.ipynb`. This will generate the files `fig3a_gou`, `fig3a_cir`, and `fig3a_tele`.
  * Panel b: run `gg230221_modelfit.ipynb` until the heading "AIC". This will generate the file `fig3b`.
  * Panel c: run `gg230221_modelfit.ipynb` from "AIC" to the end. This will generate the file `fig3c`.
* Figure 4
  * Panel a: 
    * Run `gg230227_cartoons.ipynb`. This will generate the files `fig4a_pfr_iad`, `fig4a_cstr_iad`, and `fig4a_lfr_iad`.
    * Run `gg230302_reactors.ipynb` up to the heading "Visualization". This will generate the files `fig4a_burstsize_cartoon`, `fig4a_copynumber_traj`, and `fig4a_counts_over_time`. 
  * Panel b:
    * Continue running `gg230302_reactors.ipynb` from "Visualization" to "Cell number dependence". This will generate the file `fig4b`.
  * Panel c: 
    * Continue running `gg230302_reactors.ipynb` from "Cell number dependence" to "Parameter value dependence". This will generate the file `fig4c`.
  * Panels d, e: Continue running `gg230302_reactors.ipynb` after "Parameter value dependence". This will generate the files `fig4d` and `fig4e`.
* Figure 5
  * Panel b: run `gg230131_technoisebern.ipynb`. This will generate the file `fig5b`.
  * Panels c, d: download the raw data from [Zenodo](https://zenodo.org/record/7388133), specifically `GP_2021_3_fits.tar.gz`, which contains the search data and result files. Install [*Monod*](https://github.com/pachterlab/monod/tree/dev). Run `gg230203_monod_technoise.ipynb`. This will generate the files `fig5c` and `fig5d`. 
  
Notes:
* I have tried to make the notebooks "safe," i.e., running them should take a reasonable amount of time, not perform any new computations, and not overwrite any data. 
  * This is not the case for the empty droplet code, which is slow and has to redo all of the computations from zero. (This can be revised in the future).
  * It is possible that I missed some places. If so, reach out so I can correct them. 
