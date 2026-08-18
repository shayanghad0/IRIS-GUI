# Changelog

All notable changes to this project will be documented in this file.

## [0.0.2] - 2026-08-18

### Added
- Input validation function to check if iris feature values are within realistic ranges
- Error handling for missing image file with informative error messages
- Try-except block for float conversion of input values
- Dictionary-based iris class mapping in `check_result()` function
- Input value range warnings for users entering values outside typical iris measurements

### Changed
- Improved input validation logic (replaced faulty `np.any()` check)
- Changed model selection comparison from string to integer for more robust code
- Refactored `check_result()` function to use dictionary lookup instead of multiple if-elif statements
- Fixed typo: "Logesic Regression" → "Logistic Regression"
- Fixed typo: "Accuarcy" → "Accuracy"

### Removed
- Unused `confusion_matrix` import from sklearn.metrics

### Fixed
- Fixed incorrect input validation that used `np.any(x_input) == False`
- Improved error handling for invalid numeric input entries
- Better handling of iris class prediction results
> By [Shayan Ghadamian](https://github.com/Shayanghad0/)

## [0.0.1] - 2023-09-19

### Initial Release
- GUI interface for Iris flower classification
- Support for 5 machine learning models:
  - Logistic Regression
  - K-Neighbors Classifier
  - Support Vector Classification
  - Decision Tree Classifier
  - Random Forest Classifier
- Feature input via spinbox widgets for iris measurements
- Real-time model accuracy, recall, and precision metrics display
> By [Matin Afzal](https://github.com/MatinAfzal/)