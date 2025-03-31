# Speaker Recognition System

## Overview
This repository contains a MATLAB-based implementation of a **speaker recognition system** designed to identify the speaker of a given audio file among a known set of users. The project utilizes **Mel-Frequency Cepstral Coefficients (MFCC)** for feature extraction and a **K-Nearest Neighbors (KNN)** classifier for decision-making.

## Repository Contents
```markdown
- main.m                  # Main script to launch the system
- main_v2.m               # Alternate main version with minor modifications
- eliminar_silencios.m    # Removes low-energy segments (silences)
- entramar.m              # Frames the signal and applies Hamming window
- banco_filtros.m         # Designs and applies a Mel filter bank
- freq2mel.m / mel2freq.m # Frequency scale conversions
- normalizacion_v2.m      # Normalizes feature matrices for KNN input
- kNN.m                   # KNN classification algorithm implementation
- informe_TrabajoFinal_TomasJose.pdf  # Full project report with system analysis
- Señales/                # Folder with training and test audio files
```

## MATLAB Function Summaries
- `main.m`: Controls the full speaker identification workflow.
- `eliminar_silencios.m`: Detects and removes silence using energy thresholding.
- `entramar.m`: Splits the audio into 10 ms frames and applies Hamming window.
- `banco_filtros.m`: Applies a 22-filter Mel-scale bank for spectral analysis.
- `normalizacion_v2.m`: Unifies training and test matrices and performs column-wise normalization.
- `kNN.m`: Classifies MFCC features by comparing to training data using Euclidean distance.

## Notes
- Audio samples for both training and testing are stored in the `Señales/` folder.
- The system achieves approximately **88.89%** accuracy based on cross-evaluation over 18 test cases.

## License
This project is academic and intended for educational purposes only.

## Authors
- **Tomás Ruiz Aybar**  
- **José María Rodríguez López**

