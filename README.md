# Cloud-Type Image Classification

Builds a five-class cloud classifier from the CCSN dataset using Cirrus, Cumulus, Cumulonimbus, Contrail, and Nimbostratus images. The notebook compares three transfer-learning backbones with stratified splits, class weighting, fine-tuning, and detailed evaluation.

## Workflow

1. Clone and index the CCSN image dataset.
2. Select five visually distinct cloud classes.
3. Create stratified train, validation, and test splits.
4. Train and fine-tune MobileNetV2, EfficientNetB0, and DenseNet121.
5. Compare accuracy, precision, recall, F1, confusion matrices, and training time.

## Data Requirements

- CCSN dataset cloned from `Callmewuxin/CCSN_dataset` by the notebook.

Datasets and generated artifacts are not included unless they are embedded directly in the notebook.

## Requirements

- TensorFlow/Keras
- scikit-learn
- pandas
- NumPy
- Matplotlib
- Seaborn

Install missing packages in your Jupyter or Google Colab environment before running the notebook.

## Running the Notebook

1. Open [`cloudtypeimageclassification.ipynb`](cloudtypeimageclassification.ipynb) in Jupyter Notebook or Google Colab.
2. Place any required data files in the path expected by the notebook.
3. Update local or Google Drive paths where needed.
4. Run the cells from top to bottom.

## Outputs

- Trained-model results
- Classification reports
- Confusion matrices
- Per-class metrics
- MobileNetV2 result CSV files

## Repository Contents

```text
.
|-- README.md
`-- cloudtypeimageclassification.ipynb
```

## Notes

- This repository preserves the analysis as a notebook-first educational project.
- Results may vary with dataset versions, random splits, package versions, and available hardware.
- Review file paths and runtime-specific commands before executing outside Google Colab.
