# quickml
Template for data science tasks. This folder has the following workflow:
1. A collection of notebooks for data exploration and cleaning
2. Notebook for model building
3. Model frontend via streamlit
4. Dockerized deployment

It is meant to work in the following scenarios:
1. set up an experiment on my local machine with anaconda
2. set up a run on a vm
3. run within a docker container

## Instructions
1. Rename project directory
2. Print directory structure with `apt install tree`, then `tree`. Sample below
3. Delete everything above this line when you're done

# Project title
<description>

# Set up environment
### Anaconda
```
conda create -n myenv python=3 jupyter scikit-learn pandas seaborn streamlit
conda activate myenv
```
### Docker 
'''
docker build -t myproject -f Dockerfile .
docker run -it myproject /bin/bash
'''

# 1. EDA and Data Engineering

# 2. Model Training and Evaluation

# 3. Model Packaging and Deployment
`docker build -t modeldemo .`  
`docker run -p 5000:5000 modeldemo`

# Folder structure

├── data
│   └── raw
├── models
├── notebooks
│   └── 1_EDA.ipynb
├── README.md
├── requirements.txt
├── src
│   └── utils.py
└── tests
