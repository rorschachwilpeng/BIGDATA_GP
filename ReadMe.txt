Project Introduction:
In multi-target prediction, an instance has to be classified along multiple target variables at the same time, where each target represents categories or numerical values. There are several strategies to tackle multi-target prediction problems: the local strategy learns a separate model for each target variable independently, while the global strategy learns a single model for all target variables together. Under this project, you have to first define the machine learning strategy (local or global) and then should predict (using different techniques such as multi-target regression, multi-target classification, or hierarchical multi-label classification) the driver’s behaviour according to various parameters such as weather condition, driver rush, driver well-being and so forth.

Reference and dataset:


Dataset: https://www.kaggle.com/vitorrf/cartripsdatamining

Reference paper: https://www.sciencedirect.com/science/article/pii/S003132031200430X




There are three package file:
Code:
    Which including "Global Model.ipynb" file and "Clustering.ipynb" files
    
    Global Model.ipynb:
    This is whole process for global model obtained. Which including: load data, data resampling, model training, model performance analysis in general. The output of this file is already be included in the "Data" package named as "Global_Output.csv". You can run the "Clustering" code seperately, because the result is generated already.
    
    IMPORTANT NOTE: The group used external libray "imbalance". However, due to cslinux do not defaultly install this libray. So you have to install it first, the install code was wrote in the first cell of "Gloabal Model" file. Note this plz. 
    
    Clutering.ipynb:
    This file incluing whole clustering model training process and driver pattern's prediction and its visualization. 
    
Data:
    This package including "Global_Output.csv" and "Smaller Dataset.csv" files
    
    Global_Output.csv:
    This is output file of "Global Model.ipynb". Which output the prediction of four target variable
    
    Smaller Dataset.csv:
    This is a much smaller dataset which was randomly sampled from the original dataset. The origianl dataset is not included in any file due to the submission size limitation.
   
Models:
    This package including all model you can obtained from "Code" package, you can train the model by yourself if you like :)
    
    K-Means Model: K-Means Model
    
    RandomForest_DriverRush: Random forest model, target variable is driver rush
    RandomForest_DriverWellbeing: Random forest model, target variagble is driver wellbeing
    RandomForest_RainIntensity: Random forest model, target variable is rain intensity
    RandomForest_VehicleSpeed: Random forest model, target variable is vehicle speed





    