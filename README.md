EEG Epilepsy Detection System using MATLAB GUI

The EEG Epilepsy Detection System is a MATLAB-based graphical user interface (GUI) project designed to analyze EEG signals and classify them as Normal or Epileptic using a pre-trained deep learning model. 
The system is built using MATLAB's GUIDE environment, along with pre-processed.mat data and protected.p model files.
This project is ideal for biomedical signal analysis in healthcare and academic research, especially in the field of neurological disorder detection.

Key Features:
       1. Input EEG Signal Panel:
             Users can upload EEG data files (.xls format) to visualize brain signals in the time domain. It supports real patient data inputs.
       2. Signal Preprocessing:
             The system applies bandpass filtering and Butterworth low-pass filtering to remove noise and artifacts such as EOG interference.
       3. Feature Extraction:
             It extracts statistical features like mean, variance, kurtosis, and skewness from the denoised signal to prepare input for classification.
       4. LSTM-Based Classification:
             A pre-trained LSTM (Long Short-Term Memory) model is used to detect if the EEG signal represents a normal or epileptic condition.
       5. Visual Results Display:
             • Original and Denoised EEG signal plots
             • Power Spectral Density (PSD) using Welch's method
             • Result window displaying classification outcome (Normal / Epileptic)

Project Files:
    main_pgm.m - Main GUI logic file
    main_pgm.fig - GUI design layout
    Ftrain.mat - Pre-trained features file
    LSTMtrain.p - Protected training script (non-editable)
    A LSTMtest.p - Protected prediction script (non-editable)
    EEG_data.xls, normal (1).xls, abnormal (1).xls - Sample EEG data files for testing

How to Run the Project:
    1. Install MATLAB (R2020 or later recommended)
    2. Extract all project files to a single folder
    3. Open MATLAB → Set Current Folder to the extracted folder
    4. Run the project by executing:
    ![image](https://github.com/user-attachments/assets/f61dd332-d798-4006-b760-d5ba7b2c2c13)
    
5. Upload EEG Data (.xls file) va the GUI interface
    6. Start preprocessing and classification

Requirements:
    • MATLAB with Signal Processing Toolbox
    • EEG data in .xls format
    Preloaded files: Ftrain.mat, LSTMtest.p, etc.

Outcome:
    The system will display whether the provided EEG data indicates a Normal or Epileptic condition, aiding in early detection and diagnosis of epilepsy.

Note:
    • p files are MATLAB protected files and cannot be opened or modified.
    • Make sure all files are in the same folder and the TRAIN subfolder (if used) exists as expected.
