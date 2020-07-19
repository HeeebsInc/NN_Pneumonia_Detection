# Convolutional NN: Pneumonia Detection 
![ThresholdTprFpr](PlotImages/Lung.png)

Visit [my blog](using-ai-to-detect-pneumonia-3ec4601acd07
) for a more in depth tutorial on how to create a Machine Learning/AI that predicts pneumonia given a lung x-ray image.  
## CNN Layers/Architecture
[code](CNN.ipynb)

![NNArchitecture](PlotImages/NNArchitecture.png)

## Train Test Split
[Code](Train_Test.ipynb)

All of the train, test, and pickle files can be downloaded from my [GoogleDrive](https://drive.google.com/drive/folders/1XsUTrl65JuLQvQeoSGvxqPHvZCWb6tM7?usp=sharing)
After splitting the train and test set, the class frequencies were as follows

![ClassImbalance](PlotImages/ClassImbalance.png)

## Loss and Validation
[code](CNN.ipynb)

![LossValidation](PlotImages/LossValidation.png)
## Threshold 
[code](CNN.ipynb)

![ThresholdTprFpr](PlotImages/ThresholdTprFpr.png)
## Confusion Matrix for three thresholds
[code](CNN.ipynb)

![ConfusionMatrix](PlotImages/ConfusionMatrix.png)

##Test on Google Images
To test your own images, download a lung xray with the file name being its label (normal vs. non-normal) and place it in the folder [PlotImages](PlotImages)

![GoogleTesting](PlotImages/GoogleTest.png)




