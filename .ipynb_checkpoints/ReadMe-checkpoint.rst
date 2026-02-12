VIKING Analysis
===============

:Last update: 2026-02-12 by Nishchitha S Etige

Overview
--------

This repository/folder contains notebooks used to preprocess VIKING fields and
produce analyses and figures for the VIKING ocean bottom pressure (OBP) and sea
surface height (SSH) workflow.

Notebook index
--------------

Preprocessing
^^^^^^^^^^^^^

**Nish_121825_VIKING_SSH_OBP_PVE_Preprocessing3.ipynb**
  - Reads raw VIKING data
  - Harmonizes/modifies the coordinate system for easier analysis
  - Adds a new data variable in **cm** units
  - Regrids VIKING data from a **curvilinear** grid to a **regular** grid
  - Subtracts the spatially weighted mean
  - Detrends the data
  - Exports processed VIKING output to a new ``.nc`` file

Core analyses
^^^^^^^^^^^^^

**Nish_121625_VIKING_SSH_OBP_PVE.ipynb**
  - Computes the percentage variance of ocean bottom pressure explained by
    sea surface height.

**Nish_010725_VIKING_std_diff_analysis_res_msc_raw-TM.ipynb**
  - Analyzes the standard deviation of VIKING OBP for:
    - raw
    - mean seasonal cycle (MSC)
    - residual (raw - MSC)
  - Compares results for native and 3-degree resolution.
  - Note: Due to high compute requirements, the raw/MSC/residual variance fields
    are precomputed and stored as ``.nc`` files.

Supporting computations for MSC/residual fields
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

**Nish_122925_VIKING_MSC_Res_Computation.ipynb**
  - Shows how the MSC and residual variance fields are computed.

Binned correlation analyses
^^^^^^^^^^^^^^^^^^^^^^^^^^^

**Nish_011326_VIKING_raw_bin_corr_analysis-TM.ipynb**
  - Binned correlation analysis for raw fields.

**Nish_122925_VIKING_MSC_bin_corr_analysis-TM.ipynb**
  - Binned correlation analysis for MSC fields.

**Nish_122925_VIKING_res_bin_corr_analysis-TM.ipynb**
  - Binned correlation analysis for residual fields.

Wavenumber spectra analyses
^^^^^^^^^^^^^^^^^^^^^^^^^^^

**Nish_011426_VIKING_WNS_Analysis.ipynb**
  - Main wavenumber spectra workflow.

**Nish_011426_VIKING_WNS_Analysis_Summer.ipynb**
  - Summer-only wavenumber spectra analysis.

**Nish_011426_VIKING_WNS_Analysis_Winter.ipynb**
  - Winter-only wavenumber spectra analysis.

**Nish_011426_VIKING_WNS_Analysis_GS_regimes.ipynb**
  - Wavenumber spectra analysis across Gulf Stream regimes.

**Nish_011426_VIKING_WNS_Analysis_Winter_Summer_Comp.ipynb**
  - Comparison of winter vs summer spectra.

Figures
^^^^^^^

Figure 1: VIKING vs GRACE correlation
  **Nish_121125_VIKING_GRACE_Correlation_Bin_Filter.ipynb**

Figures 2 & 3: VIKING binned standard deviation figure(s)
  **Nish_021026_VIKING_Binned_Std_Figure.ipynb**

Figure 4: VIKING binned average correlation
  **Nish_021026_VIKING_Bin_avg_cor.ipynb**
