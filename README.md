# HeartCare-Health-Monitor



# Project Overview
Internet of things (IoTs) have been part of our lives nowadays. Lots of health monitor sensors are out there to measure the health charactors of our bodies. Those devices procudce timestamped data at various sampling rate. Effectivly and efficiently using of these data can potentially help people imporve healthcare quality, detect health anormalies, and remote servies. This project is to build a near real-time sensor signal processing platform, to deal with streaming of health sensor data. It has potential application in hospital, nursing home, etc. 

# Data Source
Data is generated through a Kafka producer, which simulates 8 data sources with total of 8000 users, with a rate of 1000 /s . The basic message is in json format:
{"id":"user_id","timestamp":"event_time", "hr": heart rate number}

For example:

{"hr": 117, "id": "Susan Nathan", "time": "2016-09-23 16:11:09"}

{"hr": 103, "id": "Anthony Laura", "time": "2016-09-21 14:01:25"}

{"hr": 133, "id": "Matthew Maria", "time": "2016-09-23 16:58:55"}

{"hr": 131, "id": "Jason Rachel", "time": "2016-09-22 16:33:45"}

{"hr": 101, "id": "Susan Nathan", "time": "2016-09-20 19:12:57"}



# Spark Streaming Pipline

<img src = "https://github.com/jianshizhao/HeartCare-Health-Monitor/images/sparkstreamingpipe.png" alt = "Spark Streaming Pipline" width="500" >


Demo Presentation 
[[First Demo|https://docs.google.com/presentation/d/1flMn2waduRLvoU9rn_o9kT73yvg4pUzHyn-i1D9i91s/edit?usp=sharing]]
