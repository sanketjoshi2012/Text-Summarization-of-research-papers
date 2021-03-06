# Text Summarization of research papers
**Introduction:**

This is the github repository for the scientific team project on '**SEA: Summary Evaluation of Academic Publications with Unsupervised Methods**'. The file [**SEA_report.pdf**](https://github.com/sanketjoshi2012/Text_Summarization_ResearchPapers/blob/main/SEA_Report.pdf) is the report of the project.

The motivation behind doing this project was to check whether the unsupervised evaluation methods for text summarization task give similar results when compared with the supervised evalution methods. We have used two datasets [**CSPubSumm**](https://github.com/sanketjoshi2012/Text_Summarization_ResearchPapers/blob/main/CSPubSumm_urls.txt) and [**AIPubSumm**](https://github.com/sanketjoshi2012/Text_Summarization_ResearchPapers/blob/main/AIPubSumm_urls.txt) which includes the urls for downloading the scientific papers. The papers were downloaded by doing webscraping from **Science Direct** website. Summary generation was done using four methods **TF_IDF, TextRank, Customised TextRank with emebddings, LexRank and Ensemble (combination of TF-IDF+ TextRank)**. From the experiments, we can conclude that there is still a scope for proving our hypothesis by doing some more hyper parameter tuning and using differnt clustering methods.

We have developed this project in **Python 3** and the packages available.

**Steps:**

1. There are two text files with the list of urls [**AIPubSumm_urls.txt**](https://github.com/sanketjoshi2012/Text_Summarization_ResearchPapers/blob/main/AIPubSumm_urls.txt) and [**CSPubSumm_urls.txt**](https://github.com/sanketjoshi2012/Text_Summarization_ResearchPapers/blob/main/CSPubSumm_urls.txt). Use them to download the datasets AIPubSumm and CSPubSumm respectively.
2. There are two .ipynb files in the Notebooks folder
   1. [**Data Collection and pre-processing**](https://github.com/sanketjoshi2012/Text_Summarization_ResearchPapers/blob/main/Notebooks/Datacollection_and_preprocessing.ipynb): This notebook takes the list of urls, downloads the files and creates 8 csv files AIPubSummIntro.csv, AIPubSummOC.csv, AIPubSummAbstarct.csv, AIPubSummHighlights.csv, CSPubSummIntro.csv, CSPubSummOC.csv, CSPubSummAbstarct.csv and CSPubSummHighlights.csv.
   2. [**Generation and Evaluation**](https://github.com/sanketjoshi2012/Text_Summarization_ResearchPapers/blob/main/Notebooks/Generation_and_Evaluation.ipynb): This notebook takes the above generated 8 files and generates the summaries and evalautes the generated summaries. It also shows a few experiments that were conducted w.r.t to the validation of the geenrated summaries.

**References**
https://github.com/EdCo95/scientific-paper-summarisation#automatic-summarisation-of-scientific-papers
