Dataset description:

The dataset is composed of 350,551 minutes of data taken during 9 months totally from volunteers living in 8 different homes, using an advanced air quality sensor. 

Each data record contains:  date,  time,  temperature (in ◦C),  relative humidity (in percentage %), PM2.5 (Fine Particulate Matter in μg/m3), TVOC (Total Volatile Organic Compound in ppb), CO2 (Carbon Dioxide in ppm), CO (Carbon Monoxide in ppm), air pressure (in hPa), O3 (Ozone in ppb), NO2 (Nitrogen Dioxide in ppb). 

The raw dataset has been manipulated to add an attribute 'Activity' that can assume values 'Cooking' (class 1) or 'Other' (class 0).


Problem description:

Given the dataset described above, train a MLP for a binary-class classification probelm. The MLP has to classify if a minute belongs to the class 'Cooking' (1) or to the class 'Other' (0).


Instruction to open and run files in Colaboratory:

- On top of every file there's a link button that will open the file directly in Colaboratory. 
- Once in Colaboratory environment press Ctrl+F9 to run all.


Instructions for run main files correctily:

1. Firstly, open and run in Colaboratory the following files stored in "functions" folder:

    - MultilayerPerceptron.ipynb : this file contains a function that generates the multilayer perceptron.
    - PostProcessing_SlidingWindows.ipynb : this file contains the silding windows function for post-processing purpose.
    - CookingInstanceModality.ipynb : this file contains a function that computes the intersections between real instances of cooking and
                                      predicted instances of cooking. It also provides the computing of some metrics such as recall,                                             precision and f1-score.
    - Utils.ipynb : this file contains a function useful to compute confusion matrices and metrics such as accuracy, recall, precision 
                     and f1-score.
                                       
2. Now you can choose to run model1.ipynb (to perform a one-shot validation) or model1_cross_validation.ipynb (to perforn a cross-validation).
