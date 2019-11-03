# Sparkify
This project aims to work on a data set coming from a fictive company offering music listening service. This company is called Sparkify. Users of that service can listen music from their devices and are offered to either a free service or a paid service. The data set we will use is a server log file containing details of each user session. Sparkify would like to understand who are the user who leave the service and recognize them based on their behaviour. For that purpose we will do the following:

1. clean the data that are provided to us (server log file)
2. explore those data to familiarize with what info are available to us and how churned user are represented in the overall user population
3. build few machine learning algo that we will train to recognize who are the user who churn.
In a final step we will conclude on this exercice, with a summary of our findings.

You can read about this project in the following medium post:

https://medium.com/@piersjea/spark-ml-tells-us-who-will-churn-sparkify-audio-service-6cd494433b8c

### Requirements
I've been using the following libraries:
- PySpark
- Numpy
- Pandas
- Seaborn
- Matplotlib
- Re

### The results are as follow:
The result of the machine learning model are not in excellent range, but this can be explained by the limited number of data we used. I’ve run a cross validation with couple of parameters for the classifier. I’ve also tried other machine learning models and evaluator.

To focus on the results themself, lifetime is of course the most important feature, churn user are not long time user since they left. MaxItemSession translate the number of item in the longest session of the user. The smallest it is, the bigger the risk the user churn. Finally, giving some Thumbs Up is making user stay longer and not churn…

### Files in the repository
- Sparkify.ipynb: the jupyter notebook
- Sparkify.html : the jupyter notebook in html format
- mini_sparkify_event_data.zip: a zip file of the sparkify logs (to be unzip before running the jupyter notebook)
- README.md: this present readme information
