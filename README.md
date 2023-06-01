# test432
-> Principal component analysis (PCA) is a technique that transforms high-dimensions data into lower-dimensions 
while retaining as much information as possible.
-> One important thing to note about PCA is that it is an Unsupervised dimensionality reduction technique, 
you can cluster the similar data points based on the feature correlation between them without any supervision (or labels)

Advantages of PCA

Principal Component Analysis (PCA) is a commonly used technique in academic research, particularly in fields such as statistics,
machine learning, and data analysis. Some of the advantages of using PCA.

1)	Dimensionality reduction: One of the main advantages of PCA is its ability to reduce the dimensionality of the data while preserving most of the important information. This can be particularly useful in academic research, where datasets can be large and complex.
2)	Feature extraction: PCA can also be used for feature extraction, where the most important features of a dataset can be identified and extracted for further analysis. Feature extraction can be helpful in identifying important variables in a dataset and can also reduce the computational complexity of subsequent analyses.
3)	Visualization: PCA can also be used for data visualization, where data can be projected onto a lower-dimensional space for easier visualization and interpretation. Visualization can be helpful in identifying patterns and relationships in data and can also aid in data exploration.
4)	Data preprocessing: PCA can also be used for data preprocessing, where data can be standardized and normalized before analysis. Data preprocessing can help to reduce noise and improve the accuracy of subsequent analyses.



Disadvantages of PCA

1)	Interpretability: One of the main disadvantages of PCA is that the resulting principal components are often difficult to interpret in a meaningful way. While they may capture a large amount of variance in the data, it may not be clear what specific features or variables are being represented by each component.
2)	Data scaling: PCA is sensitive to the scaling of the data. When the data is not scaled properly, PCA may not perform optimally, and the resulting principal components may not accurately represent the variance in the original data.
3)	Outliers: PCA can be sensitive to outliers in the data. Outliers can influence the calculation of principal components and result in components that do not accurately capture the variance in the data.
4)	Correlation: PCA assumes that the variables in the data set are uncorrelated. When there is high correlation between variables, PCA may not work well, as the resulting principal components may not accurately capture the underlying structure of the data.
5)	Data distribution: PCA works best when the data is normally distributed. If the data is heavily skewed or contains extreme values, PCA may not perform optimally.
6)	Sample size: PCA may not be appropriate for small sample sizes. When the sample size is small, the resulting principal components may not accurately represent the underlying variance in the data.


Correlation
A statistical measure known as correlation expresses the direction and strength of the linear connection between two variables.

Orthogonal
Orthogonality in PCA is mathematically expressed as follows: each principal component is built to maximize the variance explained by it while adhering to the requirement that it be orthogonal to all other principal components.

Eigen Vectors
An eigenvector is a non-zero vector that only changes the magnitude not direction when subjected to a linear transformation. Mathematically, when an eigenvector is multiplied with a vector will give the product of the eigenvector and a scalar value.
+ The main components of the data are calculated using the eigenvectors. The ways in which the data vary most are represented by the eigenvectors of the data's covariance matrix. The new coordinate system in which the data is represented is then defined using these coordinates.

Covariance matrix
The covariance matrix is a p × p symmetric matrix (where p is the number of dimensions) that has as entries the covariances associated with all possible pairs of the initial variables.

STEP 1: STANDARDIZATION
The aim of this step is to standardize the range of the continuous initial variables so that each one of them contributes equally to the analysis.

STEP 2: COVARIANCE MATRIX COMPUTATION
The aim of this step is to understand how the variables of the input data set are varying from the mean with respect to each other, or in other words, to see if there is any relationship between them.

STEP 3: COMPUTE THE EIGENVECTORS AND EIGENVALUES OF THE COVARIANCE MATRIX TO IDENTIFY THE PRINCIPAL COMPONENTS
Eigenvectors and eigenvalues are the linear algebra concepts that we need to compute from the covariance matrix to determine the principal components of the data. 

STEP 4: FEATURE VECTOR
The feature vector is simply a matrix that has as columns the eigenvectors of the components that we decide to keep. This makes it the first step towards dimensionality reduction, because if we choose to keep only p eigenvectors (components) out of n, the final data set will have only p dimensions.

STEP 5: RECAST THE DATA ALONG THE PRINCIPAL COMPONENTS AXES
In this step, which is the last one, the aim is to use the feature vector formed using the eigenvectors of the covariance matrix, to reorient the data from the original axes to the ones represented by the principal components.

