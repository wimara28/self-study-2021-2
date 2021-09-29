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
  - `tweets_baby_*.csv) Keyword(育児はじめ) crawling from Twitter 2016-01-01 ~ 2021-08-31
- data_preprocess.ipynb
- tweets_crawling.ipynb
