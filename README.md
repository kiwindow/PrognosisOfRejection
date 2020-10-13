# PrognosisOfRejection
Clinical data used and computational processes in the article concerning the analysis of prognosis of rejected renal graft are stored here.

This respository has 6 files, 1 folder and this README file. 

1) renaldata.xlsx
    This is the raw clinical data. There are 211 rows of explanatory variables and 1 row of target variable at the last column.
    The sample size is 51.
    
2) renaldata.csv
    This is almost the same file as 1) excpet for the file format. To read in the renaldata file for LOOwithML.ipynb,
    you have to use this file.
    
3) LOOwithML.ipynb
    This file was made on Google Colaboratory. 
    Therefore it would be best to read this file on Google Colaboratory on the web.
    Click the file name and the contents will be shown in the GitHub.
    Then click the icon named as Open in Colab and the file will be shown in the Google Colaboratory.
    Then you can execute the program on it. To read in the dataset, you have to upload
    the renaldata.csv file in the directory on your Google drive so that the program can make an access to it.
    And you have to edit the pass for renaldata.csv in the second cell.
    The original pass was 'drive/My Drive/program/data/renaldata.csv'.
    Change this pass for the new directory where you have uploaded the dataset on Google drive.
    
4) LOOwithML.html
    This fils is saved in the HTML format. It can be read by downloading it and opening it on a web browser. 

5) LOOwitML.pdf
    This is a PDF file of LOOwithML.ipynb. You can see the contents only by clicking the file name above on the GutHut. You can also download it.
    Since its quality is not good, ipyno format or html format is recommended. 
    
6) LOOwithSRviaGP.pdf 
    This file contains the process and the result of Leave-One-Out cross validation conducted with Genetic Programming via Symbolilc regression.
   
7) AnalysisOfPredictor.nb
    This file is written in Mathematica®. So Mathematica or Wolfram Player® by Wolfram Research® is needed to read it.
    The URL of the company is https://www.wolfram.com/index.ja.html
    The Wolfram Player® is free and you can download it from https://www.wolfram.com/player/
    Just to see the AnlaysisOfPredictor.nb file, download it by clicking the file name above and open it with Wolfarm Player®.
    AnalysisOfPredictor.nb file contains the result of generating 11,540 predictive functions with DataModeler® and
    processes of distilling simple sparse model for finding dominant predictive factors.
    The caliculation was mainly done with a software, DataModeler® by Evolved Analytics® that runs on Mathematica®.
    The URL of this company is as follows: http://www.evolved-analytics.com/
    To reproduce the results in this file, DataModeler® is also needed.
    Both softwares have a free trial system.

8) AnalysisOfPredictor.pdf
    This file contains the samme contants as 5) and is saved in a PDF file.
    You can see the contants of 5) only by opening it.
    
9) DataModelerModelSets
    This file contains 11,540 models created by DataModeler®. 
    So to read in these models, DataModeler® and Mathematica® are required.
    
    
This document was written by K.I., department of blood purification, Tokyo Women's Medical University, JAPAN.
Last updated on October 14, 2020.
