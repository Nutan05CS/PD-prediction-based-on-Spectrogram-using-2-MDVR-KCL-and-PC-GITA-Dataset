Parkinson's Disease Detection from Speech Analysis
Repository Overview
This repository contains code for our comprehensive analysis of Parkinson's Disease (PD) detection using speech signals from two datasets:
•	MDVR-KCL (read text) - Unbalanced dataset
•	PC-GITA (read text) - Balanced dataset
Dataset Information
MDVR-KCL Dataset
•	Recording type: Read text
•	Class distribution: Unbalanced
•	Number of subjects: [X] PD patients, [Y] healthy controls
PC-GITA Dataset
•	Recording type: Read text
•	Class distribution: Balanced
•	Number of subjects: [X] PD patients, [X] healthy controls
Code Organization
The repository is organized into two main folders:
1. Tabular_Data_Analysis
Contains code for traditional machine learning approaches using extracted features:
•	Feature sets:
o	MFCC features
o	Spectrogram features
o	Spectral features
o	Voice quality features
o	Combined features
•	Machine learning models:
o	Random Forest (RF)
o	K-Nearest Neighbors (KNN)
o	Decision Trees (DT)
o	AdaBoost
o	Ensemble models
•	Evaluation protocols:
o	80:20 train-test split
o	5-fold cross-validation
o	10-fold cross-validation
2. Spectrogram_DL_Analysis
Contains code for deep learning approaches using spectrogram inputs:
•	Spectrogram types:
o	STFT spectrograms
o	CQT spectrograms
o	MFCC spectrograms
o	CHROMA spectrograms
o	MEL  spectrograms

•	Deep learning models:
o	Proposed attention network
o	Baseline CNN architectures
•	Evaluation protocols:
o	80:20 train-test split
o	5-fold cross-validation
o	10-fold cross-validation
o	Independent speaker evaluation
Experimental Setup
Evaluation Protocols
1.	Standard Evaluation
o	80:20 train-test split
o	5-fold cross-validation
o	10-fold cross-validation
2.	Independent Speaker Evaluation
o	Strict speaker-independent validation
o	Particularly important for clinical applicability
3.	Severity Classification
o	Attempted severity stratification (mild/moderate/severe PD)
o	Note: Limited by small sample size in severe group (n=4)
How to Use This Code
1.	For Tabular Data Analysis
o	Navigate to the Tabular_Data_Analysis folder
o	Run main_tabular.py to reproduce all experiments
o	Configuration files allow modification of:
	Feature sets
	Model parameters
	Evaluation protocols
2.	For Spectrogram DL Analysis
o	Navigate to the Spectrogram_DL_Analysis folder
o	Run main_spectrogram.py to reproduce all experiments
o	Configuration files allow modification of:
	Spectrogram parameters
	Model architectures
	Training hyperparameters
Requirements
•	Python 3.8+
•	Required packages:
o	TensorFlow 2.6+
o	scikit-learn 1.0+
o	librosa 0.9+
o	pandas 1.3+
o	numpy 1.21+
Install requirements using:

Results Reproduction
To reproduce our key results:
1.	First, run tabular data experiments
2.	Then run spectrogram experiments
3.	Severity classification
4.	Independent evaluation scripts are provided separately
Notes
•	The initial submission code is available in the main branch
•	Revised code with updates will be provided in a separate ZIP file containing:
o	Updated tabular data analysis folder
o	Updated spectrogram analysis folder
•	The ZIP file will maintain the same folder structure for consistency

