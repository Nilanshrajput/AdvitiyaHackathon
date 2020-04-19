File details :


Test data output - In Folder submission with file name submission.csv

Model File link - https://drive.google.com/drive/folders/1LvRBKB9kPmhkL1iyjrywyjaN_W9FKKFj?usp=sharing
above link contains all data and model file.

The code is made to run on Google colab so some files might need path changes

Validation acuracy of model were 100% for 2 and 99% for 1 out of 3 used model.



            - BasicEDA.ipynb : EDA of given data and making updating label names to label codes in TrainCSV
                            code - "0" - Non-Alcohol
                            code - "1" - Alcohol
                            code - "2" - Non-Autonomous Vehicle
                            code - "3" - Autonomous Vehicles
                            
             -Scrapper.ipynb :Scrap the data of patents from web, and cleans and organise the data in seprate json file for each patent.
             
             -Bert_finetuned_system.ipynb : Fine tuning Bert Model for patent classification, using Transformer Library from Hugging face and Pytorch.
                             
                             Training Details : Multiple models were trained eith diffrent token sizes, LR, Batch sizes, diffrent number of epochs.
                                                 Get good results at traing at LR = 2e-5 for 20 Epochs and another 20 epochs at LR = 3e-5(4e-5 also       
                                                 works), with max sentence length at 512, performance increases with size of sentence but GPU Memory is 
                                                 limitation.
                                                 
                                                 
                                                 
                                                 Finally 3 models are being used for prediction for scrapped data, single model also performs extremly 
                                                 well, but to increase accuracy further we are using more models.
                                                 
                                                 2 out of 3 models were showing validation accuracy of 100% and last one with 99%.
                                                 
                                                 
             -google_patent_scrapper.py: Scrapping library develped(specific for patent data scarapping) mostly by team after some initial lib code from 
                                        opensource Github account.                                
                                        
                                        
              - Drive folder containf all the data files including model weights, scrapped data in json format, CSV format cleaned data etc.
              
              
Software Stack :  Pytorch, Transformer, Beautifulsoup, Numpy, Pandas, Matplotlib

The Code was designed to run on Google colab for training and evaluation, and scrapping. The whole data was on my google drive sue to large size of Model weights, and data. SO appropraiate path changes might be required.

