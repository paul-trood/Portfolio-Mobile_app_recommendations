# Mobile App Recommendations
Google Play and Apple Store profitable mobile applications recommendations



# Google Play and Apple iOS App Recommendations

### Scenario:

We're data analysts for an app development company in the United States. Over the last five years we have established a respectably sized customer based, but there are still opportunities to grow our customer base and increase revenue. We want to develop a new app that is a stand-alone free version that our customers will enjoy. To generate revenue, we may employ in-app purchases or a subscription-based model. 

   
To minimize risks and overhead, our strategy for an app idea has three steps:

* Build a minimal Android version of the app, and add it to Google Play.
* If the app has a good response from users, we develop it further.
* If the app is profitable after six months, we build an iOS version of the app and add it to the App Store.

Since we want to develop a new app for Google Play and iOS, the app profiles we pick need to be successful for both markets.

## Method
I've done some preliminary data exploration and cleaning. I'll be using a cleaned csv file for the analysis, the file name is called `google_apps_cleaned.csv`.
We're only interested in analyzing mobile apps that are in English. The fictional company is located in the United States and only develops apps for an English-speaking audience.
The dataset that the author scraped from the Google Play store contains over 2 million rows of mobile apps. After data cleaning there remains roughly 900,000 rows of data. The following steps were taken to remove unneccessary observations:
* 7 columns dropped
* Removed missing data
* Removed apps that contain non-English characters in the `App Name` & `Developer Id` columns
* Dropped a few duplicated apps
* Filtered the current dataset to include only apps with at least 1 install and 1 rating

## Recommendations
To make sound business decisions we need to perform a few tasks during analysis:
* Review potential customer base, what are consumers downloading?
* Gauge our competition, what types of apps are our competitors developing?

## Datasets:
Raw dataset: `Google-Playstore.csv` *https://www.kaggle.com/datasets/gauthamp10/google-playstore-apps*

Cleaned dataset: `google_apps_cleaned.csv`

| Column | Description |
| --- | --- |
| `App Name` | The name of the app |
| `Category` | The category an app belongs to |
| `Rating` | Numerical rating 1 (lowest) to 5 (highest) |
| `Rating Count` | The total number of reviews |
| `Installs` | How many times a particular app is downloaded, ordinal scale |
| `Minimum Installs` | `Installs` and `Minimum Installs` are the same value except `Minimum Installs` is measured on a ratio scale  |
| `Maximum Installs` | The total maximum number of downloads of an app |
| `Free` | Whether or not an app is considered free to download/use, Boolean |
| `Price` | The current price of an app |
| `Currency` | The currency that an app is priced in |
| `Developer Id` | The name of the app developer |
| `Released` | Release date |
| `Last Updated` | The date an app was last updated by the developer |
| `Content Rating` | Appropriate audience the app is suited for |
| `Ad Supported` | Whether or not the app supports ads, Boolean |
| `In App Purchases` | Whether or not an app has in app purchases, Boolean |
| `Editors Choice` | *Some of the best Android apps of all-time on Google Play*, recommended by Google |
| `Game` | Whether or not the app category is considered a game, Boolean |


Raw dataset: `appleAppData.csv` *https://www.kaggle.com/datasets/gauthamp10/google-playstore-apps*

Cleaned dataset: `apple_apps_cleaned.csv`

| Column | Description |
| --- | --- |
| `App_Name` | The name of the app |
| `Primary_Genre` | The category an app belongs to |
| `Content_Rating` | Appropriate audience the app is suited for |
| `Released` | Release date |
| `Updated` | The date an app was last updated by the developer |
| `Version` | Latest app version |
| `Price` | The current price of an app |
| `Free` | Whether or not an app is considered free to download/use, Boolean |
| `Currency` | The currency that an app is priced in |
| `Developer` | The name of the app developer |
| `Average_User_Rating` | Numerical rating 1 (lowest) to 5 (highest) |
| `Reviews` | The total number of reviews |
