# PrognosisOfRejection

■	Clinical data and computational processes used in the article concerning the analysis of prognosis of rejected renal graft are stored here.
This repository has ten files and one folder with this README file.


◆ How to open files in the repository

・The files formatted in CSV and PDF are readable in the GitHub. 
To see them, just click their file names. 
  The PDF files can be downloaded. After clicking on the file name, another page appears and click the download button. Although a large PDF file might not be shown on GitHub properly, it can be downloaded to see it.
  
・The file with an extension of .xlsx or .nb is not shown in the GitHub. 
To see Excel® file, click on the file name to go to its own page and download it. 
  The file with the nb extension was created with Mathematica®. To see it, click on its file name to go to its own page and download it, first. Then a software, Mathematica®, Wolfram Desktop® or Wolfram Player® is needed to open it. Among them, Wolfram Player® is free. You can download it from  https://www.wolfram.com/player/ . Other software can be obtained from their developer, Wolfram Research®. Its URL is https://www.wolfram.com/index.html

・The file with an extension of .ipynb is a jupyter notebook created in the Google Colaboratory™ and written in Python™. 
  To open it, click on the file name and the contents are shown in a new page.
  To execute the codes in the file, click the button-like icon, “Open the Colab” on the top of the page. Then the file will be loaded in the Google Colaboratory™. To use Google Colaboratory™, you should have a google account, since the execution is performed on your Google Drive. Furthermore, before you evaluate the codes, the dataset, renaldata.csv, must be downloaded and uploaded in a directory of your Google Drive, like drive/My Drive/program/data/renaldata.csv. Since this file is written in Python™, it can be read and executed on a local Jupyter Notebook™ in the Python™ environment. 
  The same file is also saved as a file with an extension of .pdf or .html. The LOOwithML.pdf file can be seen by clicking the file name as already stated. The LOOwithML.html file cannot be shown in the GitHub like a web browser executes, since the raw source codes are shown on the GitHub. Therefore, to see the HTML file, click on the follow in URL address, instead: 
https://htmlpreview.github.io/?https://github.com/kiwindow/PrognosisOfRejection/blob/master/LOOwithML.html

・The folder DataModelerModelSets contains all the predictive models generated with DataModeler®. To retrieve these models and execute calculations with them, follow the commands in the Sparse modelling section in the AnalysisOfPredictor.nb file. To perform these computations, Mathematica® or Wolfram Language® and DataModeler® are needed. The former program can be obtained from Wolfram Research®, https://www.wolfram.com/index.html. The latter one can be obtained from Evolved Analytics®, http://www.evolved-analytics.com/. 
  To retrieve models in the DataModelerModelSets, this folder and a Mathematica® notebook must be saved in the same directory. Then after importing DataModeler® into the Mathematica® kernel on a Mathematica® notebook by evaluating the following command,
		Needs[“DataModeler`”]
evaluate the following code to import models as an expression of ARModels.
      ARModels = RetrieveModelSets[ ProjectName -> “PredicGraftLoss” ];


◆	Brief explanation of files in the repository

1.	renaldata.xlsx 
This is the raw clinical data. There are 211 rows of explanatory variables and 1 row of target variable at the last column. The sample size is 51.

2.	renaldata.csv 
The contents of this file is the same as those in renaldata.xlsx. To read in the renaldata file for LOOwithML.ipynb, you have to use this file.

3.	LOOwithML.ipynb 
This file was made on Google Colaboratory™. Therefore, it would be best to read this file on Google Colaboratory™ on the web in the Google Drive™. Click the file name and the contents will be shown in the GitHub. Then click the icon named as “Open in Colab” and the file will be shown in the Google Colaboratory™. Then you can execute the program on it. To read in the dataset, you have to upload the renaldata.csv file in the directory on your Google drive so that the program can make an access to it. And you have to edit the pass for renaldata.csv in the second cell of this file. The original pass is 'drive/My Drive/program/data/renaldata.csv'. Change this pass for the new directory where you have uploaded the dataset on the Google Drive™.
The contents of this file are the comparisons of classification ability between eight machine learning models, which are simple linear regression, Lasso regression, Ridge regression, logistic regression, support vector machine, random forest, XGboost and Symbolic regression via Genetic programming (SR via GP). Since the computation with SR via GP was executed on the LOOwithSRviaGP.nb file using DataModeler®, only the final result is written as for the SR via GP.

4.	LOOwithML.html 
This file is saved in the HTML format. The contents are the same as those in LOOwithML.ipynb. Although it can be read by copying it, saving it as an HTML file and opening it on a web browser, it would be convenient to assess the following URL.
https://htmlpreview.github.io/?https://github.com/kiwindow/PrognosisOfRejection/blob/master/LOOwithML.html

5.	LOOwitML.pdf 
This is a PDF file of LOOwithML.ipynb. The contents are the same as those in LOOwithML.ipynb. You can see the contents only by clicking the file name. You can also download it. Since its quality is not good, the .ipynb format or .html format is recommended.

6.	LOOwithSRviaGP.nb
This is a file written in Mathematica®. This file contains the process and the result of Leave-One-Out cross validation conducted with Genetic Programming via Symbolic regression. It can be opened with Wolfram Player® which is distributed for free. You can obtain if from https://www.wolfram.com/player/.

7.	LOOwithSRviaGP.pdf 
This file contains the process and the result of Leave-One-Out cross validation conducted with Genetic Programming via Symbolic regression.

8.	AnalysisOfPredictor.nb 
This file is written in Mathematica®. So Mathematica or Wolfram Player® by Wolfram Research® is needed to read it. The URL of the company is https://www.wolfram.com/index.ja.html The Wolfram Player® is free and you can download it from https://www.wolfram.com/player/ Just to see the AnlaysisOfPredictor.nb file, download it by clicking the file name above and open it with Wolfarm Player®. AnalysisOfPredictor.nb file contains the result of generating 11,540 predictive functions with DataModeler® and processes of distilling simple sparse model for finding dominant predictive factors. The calculation was mainly done with a software, DataModeler® by Evolved Analytics® that runs on Mathematica®. The URL of this company is as follows: http://www.evolved-analytics.com/ To reproduce the results in this file, DataModeler® is also needed. Both of them have a free trial system.

9.	AnalysisOfPredictor.pdf 
This file contains the same contents as AnalysisOfPredictor.nb and is saved in a PDF format. You can see its contents only by opening it on the GitHub. You can also download it.

10. DataModelerModelSets 
This file contains 11,540 models created by DataModeler®. To read in these models, DataModeler® and Mathematica® are required.


◇　This document was written by K.I., department of blood purification, Tokyo Women's Medical University, JAPAN. Last updated on October 17th, 2020.



