# PokerClass

## Steps to Run:
* Clone this repository to your local machine (git clone https://github.com/ajag408/PokerClass.git)
* Open Poker-Class-Prediction-Master.ipynb in an appropriate software tool (we tested with Jupyter Notebook)
* Starting from the "Preprocessing" Header (Ignore the code blocks under Collaborated via GitHub.... Header), run each code block consecutively to reproduce our results (use !pip install ____ for any missing library (replace ____ with the library name))  
  * Sample test set of 7% of the test data (70,000 sample poker hands) available at bottom of file.  Simply run the code block there to read in the sample data and evaluate on our chosen model.  
    * 7% chosen because large enough to include samples representing every class label (0-9)

  * NOTE: SMOTE strategy may throw error when our models call it depending on your version of SMOTE.  If you get the following error:
  
           TypeError: __init__() got an unexpected keyword argument 'kind'
           
   Please scroll up to the header: "Smote for Fixing Data Imbalance".  In the line starting "sc = SMOTE(...)", remove the kind parameter
