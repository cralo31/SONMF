# SONMF
Code and dataset for reproducing the results in "Topic Modeling on Triage Notes with Semi-orthogonal Non-negative Matrix Factorization".

# Dataset 
The triage data, provided by the Alberta Medical Center, is collected during the triage phase of a hospital visit in the Emergency Department. The data set contains the demographic information, medical complaints, vital readings, and documented symptoms of the patients. These documented symptoms, or triage notes, are manually typed into the system by triage nurses and is the focus of the analysis in this paper. The authors provide de-identified dataset, i.e. ‘Altered Level of Consciousness’ to the public for reproducibility and further research purposes. Other remaining datasets in the manuscript are private and has not been approved to be released to the public.

The ‘Altered Level of Consciousness’ dataset has 5220 observations (patient records) and 12 columns. The response variable used in this analysis is ‘DISPOSITION’, which is the final disposition of a patient after a doctor’s decision has been made. This is a binary variable, with a balanced ratio between Admittance (51.15%) vs. Discharge (48.85%). The ‘TriageNote’ column, which consists of the manually typed nurse notes, is the focus of this study. Additional triage information of the patients (i.e. temperature, heart rate, blood pressure, etc.) are also provided in this dataset, but they are not considered in this study. 

# Code 
The code has been divided into multiple ‘.txt’ subfiles, according to the corresponding sections in the manuscript. Each code subfile is independent from the rest except for the “code_Setup.txt” file. The first step is to run the “code_Setup.txt” file to install all the relevant packages to ensure the code runs properly. This file also provides some examples for the ‘MatrixFact’ package, which is an R package developed by the authors for the proposed method, along with other NMF methods compared in the manuscript. The ‘MatrixFact’ package can be downloaded at ‘cralo31/MatrixFact’ on Github.

All results in the simulation sections are seeded and reproducible. In addition, all results regarding the ‘Altered Level of Consciousness’ dataset are seeded and reproducible. 

Note that since the remaining triage note datasets are not available publicly, part of the manuscript is not fully reproducible. However, all the remaining datasets utilize the same analysis pipeline as the “Altered Level of Consciousness” dataset. Therefore, the provided code and dataset is sufficient for general reproducibility of our manuscript.
