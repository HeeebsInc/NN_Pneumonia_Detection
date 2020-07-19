# Convolutional NN: Pneumonia Detection 
![ThresholdTprFpr](PlotImages/Lung.png)

Visit [my blog](using-ai-to-detect-pneumonia-3ec4601acd07
) for a more in depth tutorial on how to create a Machine Learning/AI that predicts pneumonia given a lung x-ray image.  

## Data 
1. [Kaggle CoronaHack](https://www.kaggle.com/praveengovi/coronahack-chest-xraydataset)
2. [GitHub COVID Dataset](https://github.com/HeeebsInc/covid-chestxray-dataset)
3. [GoogleDrive](https://drive.google.com/drive/folders/1XsUTrl65JuLQvQeoSGvxqPHvZCWb6tM7?usp=sharing)(contains combined datasets, pickles, and csv with image paths/labels)


## CNN Layers/Architecture
[Code](CNN.ipynb)

![NNArchitecture](PlotImages/NNArchitecture.png)

## Train Test Split

All of the train, test, and pickle files can be downloaded from my [GoogleDrive](https://drive.google.com/drive/folders/1XsUTrl65JuLQvQeoSGvxqPHvZCWb6tM7?usp=sharing)

After splitting the train and test set, the class frequencies were as follows: 

[Code](Train_Test.ipynb)

![ClassImbalance](PlotImages/ClassImbalance.png)

## Loss and Validation
The model began overfitting at about 30 epochs and had F1, AUC, and ROC scores of .935, .972, and .994 respectively. [Code](CNN.ipynb)

![LossValidation](PlotImages/LossValidation.png)
![AUC_ROC](PlotImages/AUC_ROC.png)
## Threshold 
[Code](CNN.ipynb)

![ThresholdTprFpr](PlotImages/ThresholdTprFpr.png)
## Confusion Matrix for three thresholds
[Code](CNN.ipynb)

![ConfusionMatrix](PlotImages/ConfusionMatrix.png)

## Test on Google Images
To test the model on outside data, I randomly gathered 17 images from Google and used a probability threshold of .65. As you can see below, the model had a 100% True Positive rate and 56% True Negative Rate. If you download the code in my repo, there is a [folder](PlotImages) where you can try a prediction yourself. All you have to do is download the image, name the file normal or non-normal to remember its label, then run the code.

![GoogleTesting](PlotImages/GoogleTest.png)


## Future Directions
- Classify the type of Pneumonia (Viral, Fungal, etc.) 
- Use grey-scale (1D array)
- Apply SMOTE to alter class imbalances 
- Use larger images with dimensions of (96,96,3) or (204, 204,4). I initially tried using larger dimensions but my computer was too low. Having larger images can make detection more accurate as there is more detail than the latter.




