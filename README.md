<h1> <p style="font-size:32px;text-align:center"> <b>Social network Graph Link Prediction - Facebook Challenge</b> </p> </h1>

### 1. Problem statement: 
Given a directed social graph, have to predict missing links to recommend users (Link Prediction in graph)

### 2. Data Overview
Taken data from facebook's recruting challenge on kaggle https://www.kaggle.com/c/FacebookRecruiting  
data contains two columns source and destination eac edge in graph.
    - Data columns (total 2 columns):  
    - source_node         int64  
    - destination_node    int64  

### 3. Mapping the problem into supervised learning problem:
- Generated training samples of good and bad links from given directed graph and for each link got some features like no of followers, is he followed back, page rank, katz score, adar index, some svd fetures of adj matrix, some weight features etc. and trained ml model based on these features to predict link. 
- Some reference papers and videos :  
    - https://www.cs.cornell.edu/home/kleinber/link-pred.pdf
    - https://www3.nd.edu/~dial/publications/lichtenwalter2010new.pdf
    - https://kaggle2.blob.core.windows.net/forum-message-attachments/2594/supervised_link_prediction.pdf
    - https://www.youtube.com/watch?v=2M77Hgy17cg

### 4. Business objectives and constraints:  
- No low-latency requirement.
- Probability of prediction is useful to recommend highest probability links

### 5. Performance metric for supervised learning:  
- Both precision and recall is important so F1 score is good choice
- Confusion matrix

## 6. Getting Started
Start by downloading the project and run "Facebook_Link_Prediction_Models.ipynb" file in ipython-notebook.

## 7. Prerequisites
You need to have installed following softwares and libraries before running this project.
1. Python 3: https://www.python.org/downloads/
2. Anaconda: It will install ipython notebook and most of the libraries which are needed like sklearn, pandas, seaborn, matplotlib, numpy and scipy: https://www.anaconda.com/download/

## 8. Libraries
* __scikit-learn:__ scikit-learn is a Python module for machine learning built on top of SciPy.
    * pip install scikit-learn
    * conda install -c anaconda scikit-learn
    
* __networkx:__ NetworkX is a Python package for the creation, manipulation, and study of the structure, dynamics, and functions of complex networks.
    * pip install networkx
    * conda install -c anaconda networkx
    
* __nltk:__ The Natural Language Toolkit (NLTK) is a Python package for natural language processing. 
    * pip install nltk
    * conda install -c anaconda nltk
    
## 9. Authors
•	Manish Vishwakarma - Complete work  
