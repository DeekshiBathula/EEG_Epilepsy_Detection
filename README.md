EEG Epilepsy Detection System using MATLAB GUI

The EEG Epilepsy Detection System is a MATLAB-based graphical user interface (GUI) project designed to analyze EEG signals and classify them as Normal or Epileptic using a pre-trained deep learning model. The system is built using MATLAB's GUIDE environment, along with pre-processed.mat data and protected.p model files. This project is ideal for biomedical signal analysis in healthcare and academic research, especially in the field of neurological disorder detection.

Key Features:
     
   1. Input EEG Signal Panel: Users can upload EEG data files (.xls format) to visualize brain signals in the time domain. It supports real patient data inputs.
   2. Signal Preprocessing: The system applies bandpass filtering and Butterworth low-pass filtering to remove noise and artifacts such as EOG interference.
   3. Feature Extraction: It extracts statistical features like mean, variance, kurtosis, and skewness from the denoised signal to prepare input for classification.
   4. LSTM-Based Classification: A pre-trained LSTM (Long Short-Term Memory) model is used to detect if the EEG signal represents a normal or epileptic condition.
   5. Visual Results Display: • Original and Denoised EEG signal plots. • Power Spectral Density (PSD) using Welch's method. • Result window displaying classification outcome (Normal / Epileptic).

Project Files:
   1. main_pgm.m - Main GUI logic file
   2. main_pgm.fig - GUI design layout
   3. Ftrain.mat - Pre-trained features file
   4. LSTMtrain.p - Protected training script (non-editable)
   5. LSTMtest.p - Protected prediction script (non-editable)
   6. EEG_data.xls, normal (1).xls, abnormal (1).xls - Sample EEG data files for testing

How to Run the Project:

   1. Install MATLAB (R2020 or later recommended)
   2. Extract all project files to a single folder
   3. Open MATLAB → Set Current Folder to the extracted folder
   4. Run the project by executing:
    ![image](https://github.com/user-attachments/assets/f61dd332-d798-4006-b760-d5ba7b2c2c13)
   5. Upload EEG Data (.xls file) va the GUI interface
   6. Start preprocessing and classification

Requirements: • MATLAB with Signal Processing Toolbox. • EEG data in .xls format. • Preloaded files: Ftrain.mat, LSTMtest.p, etc.

Outcome: The system will display whether the provided EEG data indicates a Normal or Epileptic condition, aiding in early detection and diagnosis of epilepsy.

Note:

   1. 'LSTMtrain.p' and 'LSTMtest.p' are protected MATLAB files used for prediction logic and can't be opened directly.
   2. 'main_pgm.fig' is the GUI layout file; open with MATLAB's GUIDE or by running 'main_pgm.m'.
   3. 'Ftrain.mat' contains the pre-trained features required for EEG classification.

![image](https://github.com/user-attachments/assets/a0f62750-976d-418b-9388-6617956c3a2a)
![image](https://github.com/user-attachments/assets/690ca8e5-9877-4cb9-a2d1-8dfccc289a1c)
![image](https://github.com/user-attachments/assets/068c1876-8554-47fd-b3f0-eeb6d493fdc2)
![image](https://github.com/user-attachments/assets/4aff5cdd-0ece-44dc-a23d-f0a4c08cae59)
![image](https://github.com/user-attachments/assets/94601601-bc8a-49a3-834e-b4c96880f7a9)
![image](https://github.com/user-attachments/assets/c9970e04-fd38-4c62-a1d6-70b1643fdb21)
![image](https://github.com/user-attachments/assets/18018207-5e52-46d0-a6f1-028cbeddf443)




