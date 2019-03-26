Dataset:

The dataset contains minute-by-minute data about temperature, humidity, air pressure and different kind of gases, collected by an air quality sensor. The raw dataset has been manipulated to add an attribute 'Activity' that can assume the values 'Meal' (class 1) or 'Other' (class 0).

Problem:

Given the dataset described above, train a MLP for a binary-class classification probelm. The MLP has to classify if a minute belongs to the class 'Meal' (1) or to the class 'Other' (0).

Instructions for run main files correctily:

1. Firstly, open and run in Colaboratory the following files stored in "functions" folder:
    - MultilayerPerceptron.ipynb : this file contains a function that generates the multilayer perceptron.
    - PostProcessing_SlidingWindows.ipynb : this file contains the silding windows function for post-processing purpose.
    - CookingInstanceModality.ipynb : this file contains a function that computes the intersections between real instances of cooking and
                                      predicted instances of cooking. It also provides the computing of some metrics such as recall,                                             precision and f1-score.
    - Utils.ipynb : this file contains a function useful to compute confusion matrices and metrics such as accuracy, recall, precision 
                     and f1-score.
2. Now you can choose to run model1.ipynb (to perform a one-shot validation) or model1_cross_validation.ipynb (to perforn a cross-validation).
