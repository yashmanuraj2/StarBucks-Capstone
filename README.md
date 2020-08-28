# StarBucks-Capstone Challenge
                                        CLONE THE REPOSITORY using 'git clone https://github.com/yashmanuraj2/StarBucks-Capstone.git'
                                        Download the Transcripts file from the given Link https://drive.google.com/file/d/1NkL6wKn42av_Dsg-TFd-4lrW_JLkmfW3/view?usp=sharing
                                        Paste the transcript.json in the data folder and run the notebook
                                            
   
   Table of Contents :                  
   
   1.  Project Description
   
   2. Acknowledgement
      
   3.  AIM
   
   4 . Libraries Used
   
   5. Results 
   
   
                                  PROJECT DESCRIPTION 
   
   
   The Data contains 3  files 
   1. Profile.csv
   2.Transcripts.csv
   3.portfolio.csv
   
   The description of the files is as follows : 
#portfolio.json
id (string) - offer id
offer_type (string) - type of offer ie BOGO, discount, informational
difficulty (int) - minimum required spend to complete an offer
reward (int) - reward given for completing an offer
duration (int) - time for offer to be open, in days
channels (list of strings)
#profile.json

age (int) - age of the customer
became_member_on (int) - date when customer created an app account
gender (str) - gender of the customer (note some entries contain 'O' for other rather than M or F)
id (str) - customer id
income (float) - customer's income
#transcript.json

event (str) - record description (ie transaction, offer received, offer viewed, etc.)
person (str) - customer id
time (int) - time in hours since start of test. The data begins at time t=0
value - (dict of strings) - either an offer id or transaction amount depending on the record


                                  Acknowledgement
                                
I would Like to thanks Udacity for giving me this great project as the final Project for my nanodegree program. I would like to thank project partner Starbucks for sharing the data so that it is available to students of the classroom to study.                            
                                                   
#                                AIM OF THE PROJECT 

To create a machine learning model to predict how user responds to the offers of buy one get one free and discount offer based on users demographic variables like age gender income ,number of days since member etc.

#LIBRARIES USED 

pandas
numpy
json
matplotlib
seaborn
sklearn.grid_search 
 sklearn.neighbors import KNeighborsClassifier
sklearn.linear_model import LogisticRegression
 sklearn.tree import DecisionTreeClassifier
sklearn.svm import SVC
 sklearn.ensemble import RandomForestRegressor
 sklearn.naive_bayes import GaussianNB
 sklearn.metrics import accuracy_score,f1_score
 sklearn.model_selection import train_test_split,GridSearchCV
warnings.filterwarnings("ignore")
 
 #                                Results
 
 The model was trained on various  algorithms using default parameters( Tried  GridSeacrhCv  but was taking a lot of time and model gave a pretty good accuraacy on default parameters so 
 i chose not to use gridSearch on my model) 
 The DecisionTreeClassifier gave the best results with an accuracy of 99% and 96% on bogo and discount offers
  
