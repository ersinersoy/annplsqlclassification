# Using Artificial Neural Networks to Provide Guidance in Extending PL/SQL Programs


*Our Study is performed using GridSearchCV. Code of our study is shown on CRM_ALL_Part2.ipynb for hyperparameters below,

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

*CRM_ALL_Reproduce_Notebook.ipynb is used to reproduce our study for Single candidate on CRM-ALL Dataset

*CMS_ALL_Reproduce_Notebook.ipynb is used to reproduce our study for Single candidate on CMS-ALL Dataset

*Top_10_Results_with_Splits.xlsx file consists top 10 results for all datasets with split scores.

*All datasets(14 files) are shared as pickle dump,

    *CMS_ALL_Dataset_x.p
    *CMS_ALL_Dataset_y.p
    *CMS_T_Dataset_x.p
    *CMS_T_Dataset_y.p
    *CMS_TVPF_Dataset_x.p
    *CMS_TVPF_Dataset_y.p
    *CRM_ALL_Dataset_x.p
    *CRM_ALL_Dataset_y.p
    *CRM_T_Dataset_x.p
    *CRM_T_Dataset_y.p
    *CRM_TV_Dataset_x.p
    *CRM_TV_Dataset_y.p
    *CRM_TVPF_Dataset_x.p
    *CRM_TVPF_Dataset_y.p
