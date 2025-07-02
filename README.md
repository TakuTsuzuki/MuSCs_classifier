# MuSCs Classifier: Image Analysis Project Supplement

This repository provides the data, analysis code, and visualization notebooks used in the study: [Early and non-destructive prediction of the differentiation efficiency of human induced pluripotent stem cells using imaging and machine learning].

## Directory Structure
```
MuSCs_classifier/
├── data/                        # Raw data, intermediate data, and results
│   ├── fftfeature/              # FFT feature CSV files
│   ├── imlistD14_38.csv         # Image list CSV
│   ├── x4/                      # Raw image data (organized by day, subject, and condition)
├── src/                         # Analysis and visualization notebooks
│   ├── ①create_datatable.ipynb              # Create data tables
│   ├── ②feature_extraction_by_FFT.ipynb     # FFT feature extraction
│   ├── ③do_classification.ipynb             # Machine learning classification
│   ├── calculating_prediction_results.ipynb  # Aggregate prediction results
│   ├── check_model_validity.ipynb            # Model validity check
│   └── Visualization/                        # Visualization notebooks
└── README.md                    # This file
```

## Main Files & Notebooks

- `src/①create_datatable.ipynb`: Organize image lists and metadata
- `src/②feature_extraction_by_FFT.ipynb`: Extract features using FFT
- `src/③do_classification.ipynb`: Classification analysis using machine learning
- `src/calculating_prediction_results.ipynb`: Aggregate prediction results
- `src/check_model_validity.ipynb`: Validate model performance
- `src/Visualization/`: Visualization notebooks

## About the Data

- Raw images (tif format) are stored under `data/x4/`.
- FFT feature CSV files are in `data/fftfeature/`.
- Analysis result CSVs and log files are saved in relevant directories.

### Access to Raw Image Data (`data/x4/`)
Due to large file size and/or privacy considerations, the raw image data in `data/x4/` is **not included in this repository**.

If you wish to access the full image dataset, please contact the corresponding author:
[Hidetoshi Sakurai, hsakurai@cira.kyoto-u.ac.jp]

Requests will be considered individually.

## Reproduction Steps

1. Install all required Python packages:
   ```
   pip install -r requirements.txt
   ```

2. Run the following notebooks in order:
   1. `src/①create_datatable.ipynb`
   2. `src/②feature_extraction_by_FFT.ipynb`
   3. `src/③do_classification.ipynb`
   4. `src/calculating_prediction_results.ipynb`