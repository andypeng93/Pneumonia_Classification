# Pneumonia Image Classification
## Flatiron Mod 4 Project

**Authors**: Andy Peng

The contents of this repository detail an analysis of the module 4 project. This analysis is detailed in hopes of making the work accessible and replicable.


### Business problem:

The task is to create a model that can accurately predict whether the patient has Pneumonia or not given a patient's chest xray image. 


### Data
Our dataset comes from [Kaggle](https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia). The dataset contains three folders training, validation and testing. Each folder is filled with chest xray images used for training and testing the model that we will create.


## Methods
- Descriptive Analysis
- Modeling
- Choices made
- Key relevant findings from exploritory data analysis

## Results


#### Visual 1
<img src=./Visualizations/normal.PNG width="770">
> Normal Chest XRay

#### Visual 2
<img src=./Visualizations/pneumonia.PNG width="770">
> Pneumonia Chest XRay

#### Visual 3
<img src=./Visualizations/first_channel.PNG width="750">
> First Activation of ModelI

#### Visual 4
<img src=./Visualizations/sixth_channel.PNG width="750">
> Sixth Activation of ModelI

#### Models
<img src=./Visualizations/AUC_Score.PNG width="750">
> ROC Curve of the different Models

<img src=./Visualizations/model_table.PNG width="750">
> Model Results

* Accuracy/ Recall - Baseline Model
* Precision/F1 Score - Imbalance Model




## Recommendations:

To summarize everything above, we can see from above that

* Recall/Accuracy - ModelB
* Precicion/F1 Score/ AUC - ModelI

Our goal is to minimize the amount of patients we classify as healthy when they do indeed have Pneumonia. Therefore we would want to minimize false negatives in other words maximizing recall. Our recommendation is to stick with ModelI. Although modelB was slightly better in recall and accuracy, there was only a slight difference in the recall and accuracy score. Also ModelI did better in precision score, F1 score and AUC score. Therefore ModelI is the best model to use for predictions.

## Limitations & Next Steps

There are many things that we didn't due to lack of time and money constraints. For example, we can ask a doctor what they would look at in a chest xray image to determine whether a patient has Pneumonia or not. We could also use cross validation or gather more data to further improve our models.


### For further information
Please review the narrative of our analysis in [our jupyter notebook](./Flatiron_School_Image_Classification.ipynb) or review our [presentation](./Module4_X-Ray_Classification_(Notes).pdf)

For any additional questions, please contact andypeng93@gmail.com)


##### Repository Structure:

Here is where you would describe the structure of your repoistory and its contents, for example:

```

├── README.md                       <- The top-level README for reviewers of this project.
├── Image Classification.ipynb             <- narrative documentation of analysis in jupyter notebook
├── presentation.pdf                <- pdf version of project presentation
└── Visualization
    └── images                          <- both sourced externally and generated from code

```
