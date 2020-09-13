# Pneumonia Image Classification
## Flatiron Mod 4 Project

**Authors**: Andy Peng

The contents of this repository detail an analysis of the module 4 project. This analysis is detailed in hopes of making the work accessible and replicable.


### Business problem:

I am tasked to create a model that can accurately predict whether the patient has Pneumonia or not given a patient's chest xray image. 


### Data
Our dataset comes from [Kaggle](https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia). The dataset contains three folders training, validation and testing. Each folder is filled with chest xray images used for training and testing the model that we will create.


## Methods
- Descriptive Analysis
- Modeling
- Choices made
- Key relevant findings from exploritory data analysis

## Results


#### Visual 1
![graph1](./Visualizations/Gender.PNG)
> Gender VS Heart Disease

#### Visual 2
![graph2](./Visualizations/ChestPain.PNG)
> Chest Pain Types VS Heart Disease

#### Visual 3
![graph3](./Visualizations/Thal.PNG)
> Thalium Stress Result VS Heart Disease

#### Visual 4
![graph4](./Visualizations/Age.PNG)
> Age of Individuals VS Heart Disease

#### Visual 5
![graph5](./Visualizations/AgeMax.PNG)
> Age of Individuals VS Maximum Heart Rate

#### Models
![ROC Curve](./Visualizations/ROC1.PNG)
> ROC Curve of the different Models

![Model Results](./Visualizations/ModelResults.PNG)
> Model Results

* Accuracy/ Recall - Baseline Model
* Precision/F1 Score - Imbalance Model




## Recommendations:

To summarize everything above, we can see from above that

* Recall/Accuracy - ModelB
* Precicion/F1 Score/ AUC - ModelI

Our goal is to minimize the amount of people we classify as being normal, but they indeed do have Pneumonia. Therefore we would want to minimize false negatives in other words maximizing recall. Our recommendation is to stick with ModelI. Although modelB was slightly better in recall and accuracy, there was only a slight difference in the recall and accuracy score. Also ModelI did better in precision score, F1 score and AUC score. Therefore ModelI is the best model to use for predictions.

## Limitations & Next Steps

There are many things that we didn't due to lack of time and money constraints. For example, we can ask a doctor what they would look at in a chest xray image to determine whether a patient has Pneumonia or not. We could also use cross validation or gather more data to further improve our models.


### For further information
Please review the narrative of our analysis in [our jupyter notebook](./Heart Disease.ipynb) or review our [presentation](./SampleProjectSlides.pdf)

For any additional questions, please contact **andypeng93@gmail.com)


##### Repository Structure:

Here is where you would describe the structure of your repoistory and its contents, for example:

```

├── README.md                       <- The top-level README for reviewers of this project.
├── Image Classification.ipynb             <- narrative documentation of analysis in jupyter notebook
├── presentation.pdf                <- pdf version of project presentation
└── Visualization
    └── images                          <- both sourced externally and generated from code

```
