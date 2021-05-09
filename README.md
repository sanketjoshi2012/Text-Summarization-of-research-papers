# Text_Summarization_ovgu
**Introduction:**

This is the github repository for the scientific team project on '**SEA: Summary Evaluation of Academic Publications with Unsupervised Methods**'. The file "SEA_report.pdf" is the report of the project.

The motivation behind doing this project was to check whether the unsupervised evaluation methods for text summarization task give similar results when compared with the supervised evalution methods. We have used two datasets **CsPubSumm** and **AIPubSumm** which includes the urls for downloading the scientific papers. The papers were downloaded by doing webscraping from **Science Direct** website. Summary generation was done using four methods **TF_IDF, TextRank, LexRank and Ensemble (combination of TF-IDF+ TextRank)**. From the experiments, we can conclude that there is still a scope for proving our hypothesis by doing some more hyper parameter tuning and using differnt clustering methods.

We have developed this project in **Python 3** and the packages available.

**Steps:**

1. There are two text files with the list of urls "AIPubSumm.txt" and "CSPubSumm.txt". Use them to download the datasets AIPubSumm and CSPubSumm respectively.
2. There are two .ipynb files in the Notebooks folder
          
          1. Data Collection and pre-processing: This notebook takes the list of urls, downloads the files and creates 8 csv files AIPubSummIntro.csv, AIPubSummOC.csv, AIPubSummAbstarct.csv, AIPubSummHighlights.csv, CSPubSummIntro.csv, CSPubSummOC.csv, CSPubSummAbstarct.csv and CSPubSummHighlights.csv.
          2. Generation and Evaluation> This notebook takes the above generated 8 files and generates the summaries and evalautes the generated summaries. It also shows a few experiments that were conducted wrt to the validation of the geenrated summaries.
