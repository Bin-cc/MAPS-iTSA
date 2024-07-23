# MAPS-iTSA
We expand MAPS strategy to 1,080 FDA approved drugs for large scale target deconvolution for drug repurposing and discovery

# Files and data description
## 1. Overview descriptions of main files
![image](https://github.com/user-attachments/assets/08079b4d-a3f5-443f-9bea-e9d4cfe7249c)
+ **Figures**: Containing all main figures and supplementary figures with every sub-figures
+ **manuscript**: Including every versions of manuscripts modified by C.S.H.T and Bin Liao
+ **script**: The main part of this project which comprise core codes, input/output files, being utilized files and etc.
+ **Source data**: Experimental validation data
+ **Table**: Preliminary data information of this project (it has not been updated for long time, but latest table can be integrated from **script** file)
## 2. Details of Figures
![image](https://github.com/user-attachments/assets/d0361170-6f78-4417-94ee-120380ad7868)
+ All the Figures and supplementary figures have been listed here and the script file here involves codes used to plot some sub-figures of every figures
+ Since there are a series of update for figures, maybe part of sub-figures do not match the figures in .ai files even though they are in same files
+ The **Figure Candidate** file contain the figures that are not be performed in main/supplementary figures (part of them have actually been displayed in figures)
## 3. Details of script
![image](https://github.com/user-attachments/assets/f898440e-90f3-42f8-9232-171d04d3c491)
+ **MS_files**: Oringnal MS files derived from 480 and Lumos
+ **revised result**: Data processing and normalization result of MS data
+ **combine_group_matrix**: Pooling drug matrix of each group
+ **resource data**: All public data employed to integrate, map and calculate in house data
+ **results**: Basic calculation result (FC, pvalue and rank based on pvalue) for every drugs in each group
+ **notebooks**: Core codes for data processing, computation and visualization
+ **pkl_files**: Transition files generated during data calculations via Python
+ **output_file**: Generated key information table from data integration and calculation
+ **auto search articles**: PubMed search result for significant drug-protein pairs (fc > 0.1 & pvalue < 0.05)
+ **drugs**: Structure images of 44 drugs that identified more than 10 significant proteins
+ The .py files include all function codes called by **notebooks** code
# Utilization of codes in notebook
## 1. Environment and packages
+ All the codes are programmed by Python (version 3.11)
+ Following main packages will be implemented:
> adjust_text 0.8, Bio 1.6.2, biomart 0.9.2, imbalanced-learn 0.11.0\
> matplotlib 3.7.2, multiprocessing 0.70.14, networkx 3.1, numpy 1.24.3\
> pandas 1.5.3, pickle 0.7.5, seaborn 0.11.2, scipy 1.11.1, scikit-learn 1.3.0\
