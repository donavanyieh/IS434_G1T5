# IS434 G1T5 - Fukudonkers
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

## 1. Scrapers folder
Contains the scripts:
<ol>
  <li><b>Post_Picture_Extraction folder</b>: Contains scripts to extract and download images from Fukudon and influencer's filtered followers' 5 most recent posts. Gets image URLs from datasets in IS434_G1T5/data/followers_posts, and downloads to folders in the same directory. <b>Filtered followers</b> refers to followers who have public accounts, >5 posts, >100 followers, and [followers > (following*2.3)]</li>
<li><b>burpple_scraper.ipynb</b>: Utilize Selenium to scrape from Burrple</li>
<li><b>instagram_hashtag_scraper.ipynb</b>: Utilize Selenium and Instaloader API to scrape posts with certain hashtags from Instagram</li>
</ol>
Other sources of data (e.g. Google Review) are scraped from platforms that do not require code (e.g. PhantomBuster)

## 2. Data folder
Contains data scraped from various platforms and scrapers:
<ol>
  <li><b>CSV files</b>: Reviews from various platforms for Fukudon</li>
  <li><b>competitors folder</b>: Reviews from various platforms for competitors</li>
  <li><b>followers_posts folder</b>: 5 datasets for Fukudon and 4 identified influencers, each dataset containing the 5 most recent posts details for filtered followers. Images are extracted and downloaded from each dataset into a respective subfolders through scripts in <b>IS434_G1T5/scrapers/Post_Picture_Extraction</b></li>
  <li><b>image_json folder</b>: JSON files containing items extracted for each picture in <b>followers_posts_folder subfolders</b>. JSON file was retrieved with AWS Rekognition and S3 Browser. We identify a maximum of 10 labels with minimum confidence of 0.80, sorted by highest confidence first.
</ol>

## 3. Analysis folder
This folder contains:
<ol>
  <li><b>image_wordclouds folder</b>: Scripts to get wordclouds from json files in <b>IS434_G1T5/data/image_json folder</b>, to help identify influencer and fukudons' followers interests</li>
  <li><b>aspect_based_sentiment_analysis.ipynb</b> to perform ASBA for Fukudon and competitors (require change for data path in notebook)</li>
  <li><b>fukudon_reviews_analysis.ipynb, sticknbowls_reviews_analysis.ipynb, mentaiya_reviews_analysis.ipynb</b> performs sentiment analysis, wordclouds, and topic modelling</li>
  <li><b>post_timing_analysis.ipynb</b> analyzes best timing to post for Fukudon and its competitors</li>
  <li><b>hashtag_landscape_analysis.ipynb</b> analyzes clusters of hashtags that are popular and used frequetly together</li>
</ol>
  

## 4. Util folder
Contains files or applications required for scraping. Should remain untouched
