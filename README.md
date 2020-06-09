
# Google el ghalaba Search engine
>   simple search engine that searches the web for links or images and supports worldwide trends
## Project Structure

![project structure](images/APT.png)

## Prerequisites

* Android version above 7 (API level 23) for users
* PHP MySQL for server


## Getting started
1- creating search engine data base (MySQL)

- make sure to put the right data in the config.java class that contains:
	a) host: let it 127.0.0.1 (local host)
	b) user: the database user
	c) passwd: the log in password of the database
	d) stoppingWordsPath: the path of the file containing stopping words
	e) lastIndexingDate: the last date when the indexer run (the date that the indexer will index all data pushed after it in crawler_table).

- run **crawler** by command line :

```
javac Crawler/src/MainCrawler.java
java MainCrawler.class
```
>   or you can run MainCrawler.java from intellij/eclipse directly
- run **indexer** by command line :

```
javac Crawler/src/indexer.java
java indexer.class
```
>   or you can run indexer.java from intellij/eclipse directly
- run **popularity ranker** by command line :

```
javac Crawler/src/MainRanker.java
java MainRanker.class
```

>   or you can run MainRanker.java from intellij/eclipse directly
#
2- Run Android interface on your mobile 
> setup **AndroidInterface/final apk/google_elghalaba.apk** on your mobile
######
**OR**
>  run app directly from android studio using **AndroidInterface/source code**
![run android studio](images/Android%20Studio%20run.png)


## #Using Application :
you can view our [Demo](https://youtu.be/-2y9VjXQX2E) or follow the following instructions :

![starter](images/starter.jpg)

#### edit your server address to send requests to with the one you have :

 - your device ip -> 192.168.1.xx: 8080
 - a tunnel you are using -> xxxxxxxxxxxx.ngrok.io
#### then choose trends or search ..
# 1-Search
#### you can search with text or voice
#### **N.B. for voice make sure to leave enough space between words and at start/end of your query for good results
| ![start rec](images/start.jpg) | ![stop rec](images/stop.jpg) |

#### **the App provides you with auto complete text based on all users old queries to help you while typing
![auto complete](images/autoComplete.jpg)

#### now choose you want to search for web links or images and click ***"search"***
![choose web or images](images/choose.jpg)
## #Results :
|WEB|IMAGES |
|--|--|
|![web result 1](images/webresults1.jpg)  |![image result 1](images/imgresult1.jpg)  |
|![web result 2](images/webresults2.jpg)  |![image result 2](images/imgresult2.jpg)  |

# 2-Trends
#### just choose a country to show the trends at
![choose Country](images/chooseCountry.jpg)

#### Top 10 trends < People > of the given country are displayed
![trends results](images/trendsResults.jpg)

## Team members
[Mohamad ayman](https://github.com/TheRubick)        

[Mostafa Waleed](https://github.com/sha3er97)       

[Omar Desoky](https://github.com/OmarDesoky)        

[Kareem Osama](https://github.com/KareemOsamaSobeih) 
