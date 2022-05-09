# Therapize

**Libraries imported:**

1. For implementing bag_of_words approach:
       import random           #for random generation
       import import_ipynb    #if you are going to use multiple ipynb files to call in other
       import json            #reading/writing json files 
       import torch   
       import torch.nn as nn  #for neural network
       import numpy as np   
       import nltk   #mainly for preprocessing
       from nltk.stem.porter import PorterStemmer #just a choice of stemmer i went with, you can choose any


**Approaches:**

  1. Bag of words 
  2. GPT2-FineTuned

**Dataset Used:**

1. Bag of Words- self created corpus, saved as intents.json.
                
   what intents.json contains:
    *insert screenshot*
    
    tags for each emotion and also serving as the label here for the model
    patterns for sequences of texts, what to expect as an input, also serving as the features for the model after preparation
    responses for a list of replies the bot can randomly generate from to converse
    
2. GPT2Finetuned- already trained on 1M of corpus data [edit]
                  finetuned using a therapy_dataset.json
                  
   what therapy_dataset.json contains:
   -responses from professional psychiatrists and psychologists on questions that people may have online about mental health issues
   -user id, user's question, expert's id, expert's advice, user description etc
   -cleaned it just to make use of the **user's question and expert's advice**
   
   
   
