# Melanoma Skin Lesion Classification

Machine learning classification of melanoma from skin lesion images. The repository collects the notebooks for one project end to end: data loading and augmentation, handcrafted feature selection, dimensionality reduction, classical machine learning models, ensembles, and convolutional neural networks (CNNs), with evaluation throughout.

The notebooks refer to two datasets by the names used in the project, NHS and ALTS.

## Contents

### Data preparation
- `loading_data.ipynb` - loading and preparing the lesion image data
- `augmentation.ipynb` - image augmentation

### Feature selection and dimensionality reduction
- `feature_selection_data_visualization.ipynb`
- `univariate_feature_selection.ipynb`
- `sbs_svm_13_features.ipynb` and `sbs_nhs.ipynb` - sequential backward selection (SBS) with a support vector machine (SVM)
- `pca_nhs_1.ipynb`, `pca_analysis_nhs.ipynb` and `principal_component_analysis_nhs.ipynb` - principal component analysis (PCA)

### Classical models and ensembles
- `svm_training_nhs.ipynb` - SVM training
- `model_selection_nhs.ipynb`
- `ensemble_classifier.ipynb` and `voting_ensemble.ipynb`
- `ensemble_3_and_5_features.ipynb` - ensembles over selected feature subsets

### Deep learning
- `cnn_gridsearch.ipynb` - CNN with grid search
- `convnet_alts.ipynb`
- `convnet_alts_nhs_seg_aug.ipynb` - ConvNet on segmented, augmented images
- `visualizing_feature_maps.ipynb`

### Evaluation
- `cross_validated_predictions.ipynb`
- `confusion_matrix_reliability_curve_13_features.ipynb`
- `cohen_kappa_scores.ipynb`
- `pipeline_and_gridsearchcv_illustration.ipynb` - the overall pipeline and tuning approach

## Related repository

Handcrafted features for this project are extracted by the C++ and OpenCV code in [melanoma-feature-extraction-cpp](https://github.com/sule213/melanoma-feature-extraction-cpp).

## Notes

- Notebooks only: the lesion image datasets are not included in this repository.
- Run in a Jupyter environment with the usual scientific Python stack (NumPy, Pandas, Scikit-learn, Matplotlib) and a deep learning framework for the CNN notebooks.
