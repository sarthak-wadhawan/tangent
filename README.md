# tangent
In 1998, Yann  LeCun and others designed the framework of CNNs to classify handwritten digits for the USPS, which saved them $90m in the 1st year alone. 
This project looks at other ways to do the same.

## Techniques
- Data Visualization
- Data Exploration
- Parameter Selection using GridSearchCV which utilizes Cross Validation
- SVM
- Dimensionality Reduction (PCA - Principal Component Analysis)
- Uses binary, grsyscale images

## Functionality
It compares different cases: 
- grayscale images, binary images (black and white)
- grayscale images with dimensionality reduction using PCA
- binary images with dimensionality reduction using PCA.

The code measures accuracy, fitting time, and scoring time for each case to evaluate model performance.
