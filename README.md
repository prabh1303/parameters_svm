# Parameter Optimization of SVM
Assignment for UCS654

## About SVM and Parameter Optimization

Support Vector Machine or SVM is one of the most popular Supervised Learning algorithms, which is used for Classification as well as Regression problems. However, primarily, it is used for Classification problems in Machine Learning.

Some of the most important parameters of SVM such as kernel, C, and gamma can be changed in order to achieve a higher accuracy. This is called as Hyperparameter Tuning. 

We can perform this task using GridSearchCV for optimizing these parameters.

In this python file, I've used a Fitness Function to optimize the parameters.

## Dataset

The dataset for the project has been downloaded from the UCI Machine Learning Repository.
[https://archive.ics.uci.edu/ml/datasets/Crowdsourced+Mapping](https://archive.ics.uci.edu/ml/datasets/Crowdsourced+Mapping)

This dataset was derived from geospatial data from two sources: 1) Landsat time-series satellite imagery from the years 2014-2015, and 2) crowdsourced georeferenced polygons with land cover labels obtained from OpenStreetMap. The crowdsourced polygons cover only a small part of the image area, and are used used to extract training data from the image for classifying the rest of the image. The main challenge with the dataset is that both the imagery and the crowdsourced data contain noise (due to cloud cover in the images and innaccurate labeling/digitizing of polygons).


Number of Instances: 10546


Number of Attributes: 29

## Final Result Table

| Sample  | Best Accuracy | Best Kernel | Best Nu | Best Epsilon |
| -----   | ------------- | ----------- | ------- | ------------ |
| 1	| 0.86	| poly	  | 8.88	| 4.48 |
| 2	| 0.90	| poly	  | 4.25	| 4.11 |
| 3	| 0.91	| poly	  | 1.57	| 1.61 |
| 4	| 0.88	| poly	  | 8.37	| 0.49 |
| 5	| 0.84	| poly	  | 8.51	| 7.11 |
|	6	| 0.90	| poly	  | 1.66	| 2.77 |
| 7	| 0.87	| poly	  | 2.26	| 0.59 |
|	8	| 0.92	| poly	  | 1.35	| 3.35 |
|	9	| 0.89	| poly	  | 4.25	| 6.68 |
|	10| 0.80	| poly	  | 5.61	| 7.79 |

## Convergence Graph
![Graph](https://user-images.githubusercontent.com/73169853/233152734-12f8f0b2-fdd8-4ced-9d5c-d04362dce208.png)


## Discussion
From the above graph, we can conclude that the model is well trained and parameter have been optimized due to the less gap between training and cross-validation curve.

The graph is made for the sample which has best accuracy. Sample 8 has the best accuracy of 0.92 having kernel = Poly, Nu = 1.35 and Epsilon = 3.35.

## Written By
Name : Raunak Kumar
  
Roll No. : 102017148

Sub-Group: 3CS7
