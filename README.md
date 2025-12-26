**EE_Project_2025-26**

Short project description
This repository contains MATLAB and Simulink files to perform SST efficiency analysis using an IoT dataset, plus exported analysis reports and a simple static web report. The main artifacts are MATLAB scripts, Simulink models, dataset files, and generated result files.

Repository structure (high-level)
- Efficiency_SST.m                  — MATLAB script for efficiency calculations / analysis
- SST_Advanced_Setup.m              — MATLAB script to configure / initialize the Simulink models
- SST_Advanced_Model.slx            — Simulink model (advanced)
- SST_Basic_Model.slx               — Simulink model (basic)
- SST_Efficiency_Analysis_Report.csv — exported results
- SST_Performance_Results.mat       — MATLAB .mat results
- sst_iot_dataset_2200rows_final.xlsx — dataset used for analysis
- index.html, style.css             — static web report (view in browser)
- screenshots/*.png                 — images/screenshots of results / UI
- SST_Project.zip                   — archived project (contains project files)
- LICENSE                           — repository license

Requirements
- MATLAB (recommended: specify version, e.g., R2023a or later)
- Simulink
- (Optional) Toolboxes used (please confirm): Signal Processing Toolbox, Control System Toolbox, Statistics and Machine Learning Toolbox
- Recommended: desktop MATLAB with sufficient memory to open .slx files and large datasets

Quickstart — run analysis (example)
1. Open MATLAB.
2. Clone this repository and set MATLAB current folder to the cloned repo root:
   - git clone https://github.com/RudraCodesForU/EE_Project_2025-26.git
   - cd EE_Project_2025-26
3. Add the repo to MATLAB path (optional):
   - addpath(genpath(pwd));
4. Run the setup script to configure variables and open the Simulink model:
   - open('SST_Advanced_Model.slx');
   - run('SST_Advanced_Setup.m');
5. Run the analysis script:
   - run('Efficiency_SST.m');
6. After a run, check generated files:
   - SST_Performance_Results.mat
   - SST_Efficiency_Analysis_Report.csv

Notes:
- If you prefer the basic model, open SST_Basic_Model.slx and adapt the setup script accordingly.
- If a script expects a specific working folder, ensure MATLAB's Current Folder is repo root.

Data
- Dataset: sst_iot_dataset_2200rows_final.xlsx (and CSV export)
- Please document the dataset columns and any preprocessing steps (TODO: add dataset README or a data/ folder with schema).

Outputs
- MATLAB .mat files and CSVs with performance and efficiency results
- Screenshots and an index.html static report for quick viewing

