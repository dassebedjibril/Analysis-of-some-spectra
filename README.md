# Analysis-of-some-spectra
Here we will analyse two spectra coming from the study of Cropland Nicola and Wheat protein.

This is a regression problem where we use the spectra information **(our X)** to predict the amount of some biologocal analyte **(our Y)**. The error 
metrics obtained with an "optimal" Partial least squares regression is used as a baseline for comparisons with the CNN model. 

We will compare this model with the one where we applied data augmentation instead of correction of the baseline variations. The idea is to simulate the expected 
form of irrelevant noise (here baseline offset and slope and overall spectrum intensity), and expect the neural network to either extract features 
robust to the variations, or figure out the best corrections during training. This way we can make more efficient use of the labelled dataset. 
