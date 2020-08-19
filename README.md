# SenWave: The public sentimental analysis dataset SenWave for Covid-19 research
This dataset contains the unlabeled tweet IDs and labeled tweets used for sentimental analysis about Covid-19. The labeled tweets were organized in three languages (English and Arabic both with 10K and Chinese Weibo) while the unlabeled tweet IDs were represents with only ID to comply with Twitter’s Terms of Service in five languages (English, Arabic, Spanish, French, and Italian). In order to make use of the unlabeled data as much as possible, we utilize Google translate(https://translate.google.com/) to translate the labeled English tweets into Spanish, French, and Italian. The translated tweets are in good quality after a large number of observations. The data was collected from March 1, 2020 with Twint(https://github.com/twintproject/twint). These data is only released for non-commercial research use. 

The associated paper to this repository can be found here: SenWave: Monitoring the Global Sentiments under the COVID-19 Pandemic.

# Data Organization
The tweet IDs are organized as follows:
1) The IDs are seperated on the five languages;
2) In each language file, it stores the tweet IDs from March 1, 2020 to May 15, 2020, which are divided line by line.
3) The statistics of each language tweet IDs are shown in file lan_count.txt where first col represents the date while the second col shows the number of tweets in the corresponding day.
4) Each Txt file named as covid19_tweet_id_date.txt stores the tweet IDs.
5) The file statistics.txt counts the statistics of each language including the language, total size of this language, and the ratio in the all languages.

For the labeled tweets, we store them in the zip filefolder called labeledTweets.zip where they are organized in five CSV files where English tweets and Arabic tweets are originally annoted by experienced annotators and other three language tweets are translated with Google Translate from English tweets. The size of each kind of language tweets are all 10K. There are 11 emotions including "Optimistic", "Thankful", "Empathetic", "Pessimistic", "Anxious", "Sad", "Annoyed", "Denial", "Official report", "Surprise" and, "Joking". For Chinese Weibo dataset, 21,173 piece of data are collected by Xiaoting Lyu et al where 7 emotions are defined including "Fear", "Disgust", "Optimism", "Surprise", "Gratitude", "Sadness", and "Anger". More details about the annotated Chinese Weibo data can be found here(https://github.com/COVID-19-Weibo-data/COVID-19-sentiment-analysis-dataset-Weibo).

Note: If you want to use the labled tweets, please mail to qiang.yang[AT]kaust[dot]edu[dot]sa to get the pwd for the zip filefolder.

# Data Usage Agreement
This dataset complies with Twitter’s Terms of Service and is licensed under the Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International Public License (CC BY-NC-SA 4.0). If you use this dataset, this means that you agree with the license and term.

# Statistics Summary
The total number of tweets is 104, 830, 630. The tweets will be updated furthermore. In addition, the unlabeded Chinese Weibo data will be released soon whose size is about 1 million.
The statistics of five language tweets are shown in the following table:


|Language      |Size      |Ratio      |
| ---------- | :-----------:  | :-----------: |
|En      |68532070      |0.6537408961483872      |
|Es       |20755900       |0.1979946128340543      |
|Ar       |7957489      | 0.07590805282768977      |
|Fr       |4900973       |0.04675134547984687      |
|It       |2684198       |0.02560509271002187      |

# Citation

@article{yang2020senwave,  
  title={SenWave: Monitoring the Global Sentiments under the COVID-19 Pandemic},  
  author={Yang, Qiang and Alamro, Hind and Albaradei, Somayah and Salhi, Adil and Lv, Xiaoting and Ma, Changsheng and Alshehri, Manal and Jaber, Inji and Tifratene, Faroug and Wang, Wei and others},  
  journal={arXiv preprint arXiv:2006.10842},  
  year={2020}  
}

For Chinese Weibo dataset, please cite the paper "Sentiment Analysis on Chinese Weibo regarding COVID-19". Xiaoting Lyu, Zhe Chen, Di Wu, Wei Wang. (Citation info will be released soon.)
