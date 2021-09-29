# self-study-2021-2

논문자격시험 QE

### 2-Day Project
**Build hourly electricity consumption prediction model with provided/self-collected data**
- data/*
  - `tepco_*.txt` The hourly electricity consumption records in Tokyo (2016~current) https://www.tepco.co.jp/en/forecast/html/download-e.html
  - `weather_tokyo_*.csv` Daily weather records of Japan (2016~2021)
  - `holiday_japan_2016_2021.csv` Holiday schedule of Japan (2016~2021)
  - `d_*.csv` Keyword(葬儀を) crawling from Twitter 2016-01-01 ~ 2021-08-31 
  - `tame_*.csv` Keyword(飼いはじめ) crawling from Twitter 2016-01-01 ~ 2021-08-31 
  - `tweets_baby_*.csv` Keyword(育児はじめ) crawling from Twitter 2016-01-01 ~ 2021-08-31
  - `Total Dwellings and Residential Buildings by Stage of Construction, Started for Japan.csv` from Fred
  - `Unemployment Rate Aged 15-64 All Persons for Japan.csv` from Fred
  - `Working Age Population Aged 15-64 All Persons for Japan.csv` from Fred
- data_preprocess.ipynb
  - Preprocess tepco/weather/holiday data and tweet crawling base code.
  - Fred data were not included in this code. Additional process was done equally.
- prediction_model.ipynb
  - Build prediction model
**Model structure**
- LSTM / L1loss
- Holiday, Weather, Working people(Fred), Dwellings and Residential buildings(Fred) and Tweets that mention specific keywords were considered as variables.
- Reports from [Korea Energy Economic Institude](http://www.keei.re.kr/web_keei/d_results.nsf/0/5301D1B978CD33F7492583CE0024D40E/$FILE/%EA%B8%B0%EB%B3%B8%202018-15_%EA%B0%80%EC%A0%95%EC%9A%A9%20%EC%A0%84%EB%A0%A5%EC%86%8C%EB%B9%84%EA%B2%B0%EC%A0%95%EC%97%90%20%EC%9E%88%EC%96%B4%20%ED%96%89%EB%8F%99%EA%B2%BD%EC%A0%9C%ED%95%99%EC%A0%81%20%EC%9A%94%EC%9D%B8%20%EB%B6%84%EC%84%9D.pdf) helped create a model. 
