# Dissertation

## TODO

### 2018/5/31

* TODO:
  * [ ] Literature Review
  * [x] Latex Initial Templates

### 2018/6/1

* TODO:
  * [ ] Introduction
  * [ ] Research Structure
  * [ ] Basic Codes Using Twitter API

* Related Research:
  * Articles:
    * [ ] [Twitter Streaming and Analysis through R](http://www.indjst.org/index.php/indjst/article/viewFile/97914/75536)     `-> Twitter API`
    * [ ] [Application of Text Classification and Clustering of Twitter Data for Business Analytics](https://www.researchgate.net/publication/324360275_Application_of_Text_Classification_and_Clustering_of_Twitter_Data_for_Business_Analytics) `-> Twitter API`
    * [ ] [Twitter Data Analytics](http://tweettracker.fulton.asu.edu/tda/TwitterDataAnalytics.pdf) `-> Twitter API`
  * Tutorials:
    * [ ] [Up and running with Twitter’s API, using Python to interactively explore and analyze Twitter data](https://github.com/andersy005/Mining-Twitter) `-> Twitter API`
    * [ ] [A python wrapper around the Twitter API](https://github.com/idan/python-twitter) `-> Twitter API`

### 2018/6/3

* TODO:
  * [x] Read Article: **Trajectory Data Mining: An Overview**
* Related Research:
  * Articles:
    * [ ] [Computing with Spatial Trajectories](https://www.microsoft.com/en-us/research/wp-content/uploads/2011/11/TrajectoryComputing_Preview.pdf) `-> Trajectory Data`
    * [ ] [Trajectory Data Mining: An Overview](http://delivery.acm.org/10.1145/2750000/2743025/a29-zheng.pdf?ip=144.82.115.40&id=2743025&acc=ACTIVE%20SERVICE&key=BF07A2EE685417C5%2ED93309013A15C57B%2E4D4702B0C3E38B35%2E4D4702B0C3E38B35&__acm__=1528088154_72688ed872c009cd50b9bda55be343b5) `-> Trajectory Data`
  * Tutorials:
    * [ ] [Twitter API tutorial](http://socialmedia-class.org/twittertutorial.html) `-> Twitter API`

### 2018/6/5

* TODO:
  * [ ] Using Travel Data (TfL) to find POIs
  * [ ] Clip London PoIs of OpenStreetMap
  * [ ] Sentiment Analysis of Twitter Data Related PoIs
  * [x] Glance on geoparsepy python package

* Problems:
  1. Can not open SQL tar dumps Download <https://pythonhosted.org/geoparsepy/readme.html>

      Irror: <https://www.southampton.ac.uk/isolutions/outage-pages/personal-web-pages.page>
  
  1. ModuleNotFoundError: No module named 'config_helper'

      Because of python version??

* Related Research:
  * Python Packages:
    * [Geoparsepy](https://pypi.python.org/pypi/geoparsepy)

      Geoparsepy is a Python geoparsing library that will **extract and disambiguate locations from text**. It uses a **local OpenStreetMap database** which allows very high and unlimited geoparsing throughput, unlike approaches that use a third-party geocoding service (e.g. Google Geocoding API).

      Geoparsing included the following features :
      * **token expansion** using location name variants (i.e. OSM multi-lingual names, short names and acronyms)
      * **token expansion** using location type variant88s (e.g. street, st.) 
      * **token filtering** of single token location names against WordNet (non-nouns), language specific stoplists and peoples first names (nltk.corpus.names.words()) to reduce false positive matches
      * **prefix checking** when matching in case a first name prefixes a location token(s) to avoid matching peoples full names as locations (e.g. Victoria Derbyshire != Derbyshire)

      **Location disambiguation** is based on an evidential approach, with evidential features detailed below in order of importance:
      * **token subsumption**, rejecting smaller phrases over larger ones (e.g. ‘New York’ will prefer [New York, USA] to [York, UK])
      * **nearby parent region**, preferring locations with a parent region also appearing within a semantic distance (e.g. ‘New York in USA’ will prefer [New York, USA] to [New York, BO, Sierra Leone])
      * **nearby locations**, preferring locations with closeby or overlapping locations within a semantic distance (e.g. ‘London St and Commercial Road’ will select from road name choices with the same name based on spatial proximity)
      * **nearby geotag**, preferring locations that are closeby or overlapping a geotag
      * **general before specific**, rejecting locations with a higher admin level (or no admin level at all) compared to locations with a lower admin level (e.g. ‘New York’ will prefer [New York, USA] to [New York, BO, Sierra Leone]

    [geoparsepy user documentation](https://pythonhosted.org/geoparsepy/readme.html)

    [geoparsepy API documentation](https://pythonhosted.org/geoparsepy/index.html)

    [Github Similar Example](https://github.com/buyuhuang/cliowire-bots)
  
  * Articles:
    * [ ] [Geoparsing and Geosemantics for Social Media: Spatio-Temporal Grounding of Content Propagating Rumours to support Trust and Veracity Analysis during Breaking News](http://delivery.acm.org/10.1145/2850000/2842604/a16-middleton.pdf?ip=144.82.115.188&id=2842604&acc=ACTIVE%20SERVICE&key=BF07A2EE685417C5%2ED93309013A15C57B%2E4D4702B0C3E38B35%2E4D4702B0C3E38B35&__acm__=1528231885_048e3235cf7afab80aa9bd4326986742)
    * [ ] [Real-Time Crisis Mapping of Natural Disasters Using Social Media](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=6692841)

