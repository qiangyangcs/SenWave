# SenWave: The public sentimental analysis dataset SenWave for Covid-19 research
This dataset contains the unlabeled tweet IDs and labeled tweets and Weibo used for sentimental analysis about Covid-19. The labeled tweets were organized in three languages (English and Arabic both with 10K and Chinese Weibo with about 22K) while the unlabeled tweet IDs were represented with only IDs to comply with Twitter’s Terms of Service and Weibo's Terms of Service in six languages (English, Arabic, Spanish, French, and Italian in Tweets and Chinese in Weibo data). In order to make use of the labeled data as much as possible, we utilize Google translate(https://translate.google.com/) to translate the labeled English tweets into Spanish, French, and Italian. The translated tweets are in good quality after a large number of observations. The twitter data was collected from March 1, 2020 with Twint(https://github.com/twintproject/twint) while the Weibo data was collected from January 10. These data is only released for non-commercial research use. 

*********GOOD NEWS*************
 Up to now, there are more than 68 users from 20 countries such as USA, China, India, Singapore, Italy, Saudi Arabia, etc., applying for the usage of our dataset and 26 citations for the arxiv paper.

The associated paper to this repository can be found here: SenWave: Monitoring the Global Sentiments under the COVID-19 Pandemic.

# Data Organization
The tweet IDs are organized as follows:
1) The IDs are seperated on the five languages;
2) In each language file, it stores the tweet IDs from March 1, 2020 to May 15, 2020, which are divided line by line.
3) The statistics of each language tweet IDs are shown in file lan_count.txt where first col represents the date while the second col shows the number of tweets in the corresponding day.
4) Each Txt file named as covid19_tweet_id_date.txt stores the tweet IDs.
5) The file statistics.txt counts the statistics of each language including the language, total size of this language, and the ratio in the all languages.

For the labeled tweets, we store them in the zip filefolder called labeledTweets.zip where they are organized in five CSV files where English tweets and Arabic tweets are originally annoted by experienced annotators and other three language tweets are translated with Google Translate from English tweets. The size of each kind of language tweets are all 10K. There are 11 emotions including "Optimistic", "Thankful", "Empathetic", "Pessimistic", "Anxious", "Sad", "Annoyed", "Denial", "Official report", "Surprise" and, "Joking". For Chinese Weibo dataset, 21,173 piece of data are collected by Xiaoting Lyu, Prof. Huang (Tsinghua Universityet) et al. where 7 emotions are defined including "Fear", "Disgust", "Optimism", "Surprise", "Gratitude", "Sadness", and "Anger". More details about the annotated Chinese Weibo data can be found here(https://github.com/COVID-19-Weibo-data/COVID-19-sentiment-analysis-dataset-Weibo).

Note: If you want to use the labled tweets, please mail to qiang.yang[AT]kaust[dot]edu[dot]sa to get the pwd for the zip filefolder.

# Data Usage Agreement
This dataset complies with Twitter’s Terms of Service. If you use this dataset, this means that you agree with the license and term of Twitter.

# Statistics Summary
The total number of tweets is 104, 830, 630 (about 105M+ plusing Chinese data). The tweets will be updated furthermore. In addition, the unlabeded Chinese data will be released soon whose size is about 1 million.
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

@article{zhang2021rise,
  title={Rise and fall of the global conversation and shifting sentiments during the COVID-19 pandemic},
  author={Zhang, Xiangliang and Yang, Qiang and Albaradei, Somayah and Lyu, Xiaoting and Alamro, Hind and Salhi, Adil and Ma, Changsheng and Alshehri, Manal and Jaber, Inji Ibrahim and Tifratene, Faroug and others},
  journal={Humanities and Social Sciences Communications},
  volume={8},
  number={1},
  pages={1--10},
  year={2021},
  publisher={Palgrave}
}

For Chinese Weibo dataset, please cite the paper "Sentiment Analysis on Chinese Weibo regarding COVID-19". Xiaoting Lyu, Zhe Chen, Di Wu, Wei Wang. (Citation info will be released soon.)

Here, we thanks for the contribution of Prof. Huang in Tsinghua University.

# Scope of data usage

Note that our dataset and analyses can be applied to similar tasks or events which need the fine-grained emotions, like stock market forecast, and public opinion mining.  Comparative studies can also be done to analyze the difference between COVID-19 Twitter data and regular social media data.
