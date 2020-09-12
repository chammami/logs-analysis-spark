# Logs analysis with Spark

This repository hosts an application project to practice data wrangling and modeling using Apache Spark. 

The main objective of this project is to protect a web server namely [Link](http://www.almhuette-raith.at/) from bot attacks by using a mixed of domain knowledge and Machine Learning techniques.

The project structure is detailed below.
To reproduce my work, you can follow the steps detailed below.


Thank you for considering examining my work and application !

```bash
├── data
│   ├── processed						# Directory for processed files
│   │   ├── cleaned_logs					## Parsed logs
│   │   │   ├── *.parquet
│   │   ├── featurized_logs					## Engineered features
│   │   │   ├── *.parquet
│   │   └── labeled_df						## labeld features
│   │       ├── *.parquet
│   └── raw							# Directory for raw logs file
│       ├── access.log						## Deleted to save storage space
│       └── parsing_stats.csv					## Checkin parsing stats
├── docs
│   └── figs
│       ├── data_pipeline.png
├── notebooks
│   ├── Logs analysis - exploratory data analysis.ipynb
│   ├── Logs analysis - Features Engineering.ipynb
│   ├── Logs analysis - Machine Learning.ipynb
│   └── Logs analysis - preprocessing.ipynb
├── README.md
└── requirements.txt
```


To run the entire project: Follow these steps:

1 - install pyspark following this link: 
https://medium.com/@GalarnykMichael/install-spark-on-ubuntu-pyspark-231c45677de0

2- Then upgrade pip
   ```$ sudo pip install --upgrade pip```
   
3- Install conda
     ```$ pip install conda```
     
4 - Create a conda env with requirements.txt file
    ```$ conda --name myenv --file requirements.txt```
    
5 -activate conda env:
    ```$ conda activate myenv```
    
6 -Finally, start jupyter with Spark Support:
   ```$ snotebook```

