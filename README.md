# Using Artificial Neural Networks to Provide Guidance in Extending PL/SQL Programs

This project involves the creation of an artificial neural network model to automatically predict the correct placement of a new PL/SQL object among one of the existing schemas. The model uses dependencies among the software and database objects as features for training. Then, given a new object and the list of other objects it uses, the network can predict the schema, where the object should be included. 

This repository includes executable Python scripts in the form of Jupiter notebooks for creating the model, optimizing the hyperparameters of the model via grid search, training and validating the model. It also includes a set of datasets used for training and validating the model as well as the obtained results.

Grid search for optimizing the hyperparameters is performed by using the *Scikit-Learn-GridSearchCV* module. The corresponding code for one of the optimized parameter sets (as listed below) is provided in *CRM_ALL_Part2.ipynb* and *CMS_ALL_Part2.ipynb*. 

      'hidden_layer_sizes': 
        (50, 50),
        (50, 100),
        (50, 150),
        (50, 200),
        (50, 250),
        (50, 500),
        (50, 750),
        (50, 1000),
        (50, 1250),
        (50, 1500),
        (50, 1750),
        (50, 2000),
        (50, 2250),
        (50, 2500),
        (50, 2750),
        (50, 3000)
       'activation': 'logistic', 'tanh'
       'alpha': 0.0001, 0.0005, 0.001, 0.0015, 0.002

The following two files can be used for reproducing our study and results.
- *CRM_ALL_Reproduce_Notebook.ipynb* is used for performing prediction based on the *CRM-ALL* dataset (*CRM_ALL_Dataset_x.p*).
- *CMS_ALL_Reproduce_Notebook.ipynb* is used for performing prediction based on the *CMS-ALL* dataset (*CMS_ALL_Dataset_x.p*).

*Top_10_Results_with_Splits.xlsx* includes top 10 results for all datasets with split scores.

All datasets (14 files) are shared as pickle dump with the filenames listed as follows.

- *CMS_ALL_Dataset_x.p*
- *CMS_ALL_Dataset_y.p*
- *CMS_T_Dataset_x.p*
- *CMS_T_Dataset_y.p*
- *CMS_TVPF_Dataset_x.p*
- *CMS_TVPF_Dataset_y.p*
- *CRM_ALL_Dataset_x.p*
- *CRM_ALL_Dataset_y.p*
- *CRM_T_Dataset_x.p*
- *CRM_T_Dataset_y.p*
- *CRM_TV_Dataset_x.p*
- *CRM_TV_Dataset_y.p*
- *CRM_TVPF_Dataset_x.p* 
- *CRM_TVPF_Dataset_y.p*

# About Python and Python Library Versions Used in this Study

Please find Python and used python libraries versions in this study below,

- *The Python version is 3.6.3.

- Python Libraries,

      - *The pickle version is 4.0.
      - *The numpy version is 1.13.3.
      - *The scikit-learn version is 0.19.1.
      - *The pandas version is 0.20.3.

# How To Run
1. Install anaconda (It will install all necessary tools and libraries for you)
      https://www.anaconda.com/products/individual
2. Download all the files on github to your local storage
3. Type "jupyter notebook" in command line when same path with files
