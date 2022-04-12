# Fukudonkers
Project for IS434 - Social Analytics & Applications<br><br>
Supervisor: Professor Kyong<br>
Sponsor: Fukudon<br>
Team Members: Ang Heng Di, Teh Rui Ning Shayna, Tan Yeo Shi Lee, Kylie Tan Jia Yun, Goh Tse Ting Claire, Yieh Yuheng
<br>
## Pre-requisites
Python 3.10

## Set-up dependencies
Run in root directory:
```python
pip install -r requirements.txt
```

## Directory information
This repository contains 4 sub-folders: <b>(i) scrapers, (ii) data, (iii) analysis, (iv) util</b>.<br>
The workflow of this project is as follows:<br>
<ol>
  <li>Scrape data from scraping scripts in <i>scrapers</i> folder</li>
  <li>Save data in <i>data</i> folder</li>
  <li>perform analysis from <i>analysis</i> folder</li>
</ol>

## 1. Scrapers folder
Contains the scripts:
<ol>
<li><b>burpple_scraper.ipynb</b>: Utilize Selenium to scrape from Burrple</li>
<li><b>instagram_hashtag_scraper.ipynb</b>: Utilize Selenium and Instaloader API to scrape posts with certain hashtags from Instagram</li>
<li><b>IG_scraper.ipynb</b>: Utilize Instaloader API to </li>
</ol>
Other sources of data (e.g. Google Review) are scraped from platforms that do not require code (e.g. PhantomBuster)

## 2. Data folder
Contains data scraped from various platforms and scrapers<br><br>
<b> gg </b>

## 3. Analysis folder
This folder contains:
<ol>
  <li><b>aspect_based_sentiment_analysis.ipynb</b> to perform ASBA for Fukudon and competitors (require change for data path in notebook)</li>
  <li><b>fukudon_reviews_analysis.ipynb, sticknbowls_reviews_analysis.ipynb, mentaiya_reviews_analysis.ipynb</b> performs sentiment analysis, wordclouds, and topic modelling</li>
  <li><b>post_timing_analysis.ipynb</b> analyzes best timing to post for Fukudon and its competitors</li>
  <li><b>hashtag_landscape_analysis.ipynb</b> analyzes clusters of hashtags that are popular and used frequetly together</li>
</ol>
  

## 4. Util folder
Contains files or applications required for scraping. Should remain untouched
