# TweetMap

Real Time Sentiment analysis of tweets, visualized over world map using  AWS Cloud using Python, Django and Twitter Streaming API.
This application uses:
- Google Map API: for plotting the tweets on a map
- Elastic Search: for efficient searching of tweets based on keywords stored in JSON format on AWS ElasticSearch Service
- Amazon SQS: A queueing service to store the streamed tweets making them available for consumption
- Amazon SNS: A notification service that notifies the subscriber of new available tweets.

Application Architecture:
![Alt text](TwittMap/arch.JPG?raw=true "Application Architecture")

Web Application Screenshot:
![Alt text](TwittMap/appscreen.JPG?raw=true "Screenshot")


This application is created using Python Django framework and hosted on AWS BeanStalk.

Steps to run the application:

- Download the project
- Update Twitter and AWS keys in config.ini file.
- Run manage.py file --> python manage.py runserver
- To stream new tweets run TwitterStreamer.py and SentimentAnalyzer.py
- Access the application in browser --> http://localhost:8000
