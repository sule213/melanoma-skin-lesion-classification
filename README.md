# Melanoma Skin Lesion Classification

Machine learning classification of melanoma from skin lesion images. The repository collects the notebooks for one project end to end: data loading and augmentation, handcrafted feature selection, dimensionality reduction, classical machine learning models, ensembles, and convolutional neural networks (CNNs), with evaluation throughout.

The notebooks refer to two datasets by the names used in the project, NHS and ALTS.

## Contents

### Data preparation
- `Loading data MELANOMA.ipynb` - loading and preparing the lesion image data
- `Augmentation.ipynb` - image augmentation

### Feature selection and dimensionality reduction
- `Feature Selection and Data Visualization.ipynb`
- `Univariate Feature Selection.ipynb`
- `(SBS)-SVM-NHS-13.ipynb` and `SBS NHS.ipynb` - sequential backward selection (SBS) with a support vector machine (SVM)
- `(PCA)-NHS-1.ipynb`, `PCA Analysis NHS.ipynb` and `Principal component analysis (NHS).ipynb` - principal component analysis (PCA)

### Classical models and ensembles
- `SVM NHS Training.ipynb` - SVM training
- `Model Selection NHS.ipynb`
- `Ensemble Classifier.ipynb` and `Voting Ensemble.ipynb`
- `3 and 5 Ensemble 5 features-Copy1.ipynb` - ensembles over selected feature subsets

### Deep learning
- `CNN MELANOMA-GridSearch.ipynb` - CNN with grid search
- `ConvNet ALTS-MELANOMA.ipynb`
- `ConvNet aLTS-NHS-SEG-AUG.ipynb` - ConvNet on segmented, augmented images
- `Visualizing Feature Maps (Sample Positive).ipynb`

### Evaluation
- `Cross-Validated Predictions.ipynb`
- `Confusion matrix and Reliability Curve 13 Features.ipynb`
- `Cohen Kappa Scores.ipynb`
- `Illustration of Pipeline and GridSearchCV.ipynb` - the overall pipeline and tuning approach

## Related repository

Handcrafted features for this project are extracted by the C++ and OpenCV code in [melanoma-feature-extraction-cpp](https://github.com/sule213/melanoma-feature-extraction-cpp).

## Notes

- Notebooks only: the lesion image datasets are not included in this repository.
- Run in a Jupyter environment with the usual scientific Python stack (NumPy, Pandas, Scikit-learn, Matplotlib) and a deep learning framework for the CNN notebooks.
