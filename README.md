# CDAC Hackathon
## COVID-19 LITERATURE ANALYSIS AND SUMMARIZATION PLATFORM

### Steps to run the project:

* **Requirements:**<br>
  1. python: version 3.7.x
  2. npm: version 6.13.4
  3. node: version 12.16.0
  4. pip and pipenv
 
* **Steps:**
  1. Clone the repository using<br> **git clone https://github.com/tanmaypardeshi/CDAC-Hackathon.git**
  2. Use command **pipenv shell** to activate pipenv
  3. For the first time, use **pipenv install** to install all dependencies<br>
  This will only be for the first time to install the packages.
  4. Use **npm i** for the first time to install all node modules for React.
  5. To run the flask server use **python run.py**
  6. Run **npm start** to start development server and use the platform while keeping 
  the flask server running as well
 
  
### Documentation about the files in the repository

**1. Covid_Data.json:** Dataset in the json format.<br> 

Follow the following steps to open the file:

```
import json
f=open ('Covid_Data.json') 
data = json.load(f)
print(data)
```

**2. Data_Covid.csv:** Dataset created by using Kaggle open Research data. It is advisable to use pd.read_csv in order to open the file, as the size of the file is too large

```
import pandas as pd
data=pd.read_csv('Data_Covid.csv') 
print(data)
```

**3. glove:** Embeddings used to create the dataset.

**4. data_script.ipynb:** The script written in order to extract data from the source data in the required format

**5. Summarizer.py:** Makes use of the TextRank algorithm to summarize the input Biomedical Text.


### Research papers referred while working for the TextRank algorithm:
#### (Click on the links to open the research paper)

* [Unsupervised Text Summarization Using Sentence Embeddings](https://www.cs.utexas.edu/~asaran/reports/summarization.pdf):

    This research paper explains the process of text summarization using unsupervised methods. It is done by clustering sentence embeddings trained to embed paraphrases near each other. 
* [Application and analysis of text summarization for biomedical domain content](http://cs229.stanford.edu/proj2019spr/report/77.pdf):
    
    Application and analysis of text summarization for biomedical domain content 
* [Supervised Machine Learning for Extractive Query Based Summarisation of Biomedical Data](https://www.aclweb.org/anthology/W18-5604.pdf):

This paper explores the impact of several supervised machine learning approaches for extracting multi-document summaries for given queries. It compares classification and regression approaches for query-based extractive summarisation using data provided by the BioASQ Challenge.
* [Information Retrieval as Statistical Translation](Information Retrieval as Statistical Translation):

This paper proposes a new probabilistic approach to information retrieval based upon the ideas of statistical machine translation. The main approach is a statistical model on how a document can be translated into a query.


#### [Click here to open the text file used in the screen recording](Crystallization and preliminary crystallographic study of Feline infectious peritonitis virus main protease in complex with an inhibitor.txt)

### Snippets of the platform:

![clasp_1](/screenshots/clasp_1.png)
![clasp_2](/screenshots/clasp_2.png)
![clasp_3](/screenshots/clasp_3.png)
![clasp_4](/screenshots/clasp_4.png)
![clasp_5](/screenshots/clasp_5.png)
![clasp_6](/screenshots/clasp_6.png)
 
