# Accel_Parkinson_Classification
Using Smart device tri-axial accelrometer readings to predict Parkinsons symptom severity

Input Data from the Accelerometer sensor should contain the following channels:
  (Timestamp, X Acceleration, Y Acceleration, Z Acceleration)

For the purposes of this work, a single user's data (User 1004) has been setup for full feature extraction and modelling, as this can be a lengthy process. If there are any further requests or data requirements please contact Kieran.Grennan3@mail.dcu.ie

Python Notebooks have already been run with Google Colab and the Git repo shows extracted features with EDA and modelling evalution plots and results.

# Feature Extraction workflow:
  1. Open Feature_Extraction.ipynb
  2. Mount Google Drive (code block ln[1])
  2. Edit 'savedir' to shared link provided by email ('Data' folder was shared)
  3. Rerun code block ln[1] to link saved directory
  4. Now step through and run each block to load the pyhton libraries for DSP and data handling, setup the results directory and define all processing functions.
  5. Run 'EDA' section if plots and visualizations of features are desired.
  6. Finally run 'Processing & Saving loop' to extract these features from raw signal data
  
# Modelling Pipeline:
  1. Open Modelling_Pipeline.ipynb
  2. Mount Google Drive (code block ln[1])
  2. Edit 'savedir' to shared link provided by email ('Data' folder was shared)
  3. Rerun code block ln[1] to link saved directory
  4. Now step through and run each block to load the pyhton libraries for ML modelling, data handling, setup the results directory and define all custom processing functions.
  5. Progres through the blocks until all functions are setup.
  6. Run 'Load user data' block ln[177] and begin to prepare the feature set for modelling
  7. If process time is of interest then only run 'PCA' block of the 'Dimensionality reduction' section.
  8. Finally process the features and model each section with the proposed model - Random Forest.
  9. Observe the evaluation results with the plots and output metrics.
  
# Citation Information
The Modelling pipeline notably mentions and references some feature extraction functions which have been adapted for use in the current project. The original functions for Gait and Tremor clasisifcation and feature extraction is available at: https://github.com/NikhilMahadevan/analyze-tremor-bradykinesia-PD.git
