# Dissertation

<!-- TOC depthFrom:2 -->

- [2018-5-31](#2018-5-31)
    - [TODO](#todo)
- [2018-6-1](#2018-6-1)
    - [TODO](#todo-1)
    - [Related Research](#related-research)
        - [Articles](#articles)
        - [Tutorials](#tutorials)
- [2018-6-3](#2018-6-3)
    - [TODO](#todo-2)
    - [Related Research](#related-research-1)
        - [Articles](#articles-1)
        - [Tutorials](#tutorials-1)
- [2018-6-5](#2018-6-5)
    - [TODO](#todo-3)
        - [Problems](#problems)
    - [Related Research](#related-research-2)
        - [Python Packages](#python-packages)
    - [Articles](#articles-2)
- [2018-6-13](#2018-6-13)
    - [Datasets](#datasets)
        - [Twitter API](#twitter-api)
        - [TfL Open Data](#tfl-open-data)
        - [Met Office](#met-office)
        - [Ordnance Survey](#ordnance-survey)
    - [Articles](#articles-3)
        - [Profiling people and places for targeted advertising](#profiling-people-and-places-for-targeted-advertising)
        - [Modernising the National Travel Survey](#modernising-the-national-travel-survey)
    - [Blogs](#blogs)
        - [Me, Geolocated on Twitter](#me-geolocated-on-twitter)
    - [Python Packages](#python-packages-1)
        - [Tweepy](#tweepy)
- [2018-6-14](#2018-6-14)
    - [TODO](#todo-4)
- [2018-6-26](#2018-6-26)
    - [TODO](#todo-5)
- [2018-07-04](#2018-07-04)
    - [ogr2ogr](#ogr2ogr)
    - [geoparsepy](#geoparsepy)
    - [TODO](#todo-6)

<!-- /TOC -->

## 2018-5-31

### TODO
  
- [ ] Literature Review
- [x] Latex Initial Templates

## 2018-6-1

### TODO

- [ ] Introduction
- [ ] Research Structure
- [ ] Basic Codes Using Twitter API

### Related Research
  
#### Articles

- [ ] [Twitter Streaming and Analysis through R](http://www.indjst.org/index.php/indjst/article/viewFile/97914/75536)     `-> Twitter API`
- [ ] [Application of Text Classification and Clustering of Twitter Data for Business Analytics](https://www.researchgate.net/publication/324360275_Application_of_Text_Classification_and_Clustering_of_Twitter_Data_for_Business_Analytics) `-> Twitter API`
- [ ] [Twitter Data Analytics](http://tweettracker.fulton.asu.edu/tda/TwitterDataAnalytics.pdf) `-> Twitter API`

#### Tutorials

- [ ] [Up and running with Twitter’s API, using Python to interactively explore and analyze Twitter data](https://github.com/andersy005/Mining-Twitter) `-> Twitter API`
- [ ] [A python wrapper around the Twitter API](https://github.com/idan/python-twitter) `-> Twitter API`

## 2018-6-3

### TODO

- [x] Read Article: **Trajectory Data Mining: An Overview**

### Related Research
  
#### Articles

- [ ] [Computing with Spatial Trajectories](https://www.microsoft.com/en-us/research/wp-content/uploads/2011/11/TrajectoryComputing_Preview.pdf) `-> Trajectory Data`
- [ ] [Trajectory Data Mining: An Overview](http://delivery.acm.org/10.1145/2750000/2743025/a29-zheng.pdf?ip=144.82.115.40&id=2743025&acc=ACTIVE%20SERVICE&key=BF07A2EE685417C5%2ED93309013A15C57B%2E4D4702B0C3E38B35%2E4D4702B0C3E38B35&__acm__=1528088154_72688ed872c009cd50b9bda55be343b5) `-> Trajectory Data`

#### Tutorials

- [ ] [Twitter API tutorial](http://socialmedia-class.org/twittertutorial.html) `-> Twitter API`

## 2018-6-5

### TODO

- [ ] Using Travel Data (TfL) to find POIs
- [ ] Clip London PoIs of OpenStreetMap
- [ ] Sentiment Analysis of Twitter Data Related PoIs
- [x] Glance on geoparsepy python package

#### Problems

1. Can not open SQL tar dumps Download <https://pythonhosted.org/geoparsepy/readme.html>

    Irror: <https://www.southampton.ac.uk/isolutions/outage-pages/personal-web-pages.page>

1. ModuleNotFoundError: No module named 'config_helper'

    Because of python version??

### Related Research
  
#### Python Packages

- [Geoparsepy](https://pypi.python.org/pypi/geoparsepy)

  Geoparsepy is a Python geoparsing library that will **extract and disambiguate locations from text**. It uses a **local OpenStreetMap database** which allows very high and unlimited geoparsing throughput, unlike approaches that use a third-party geocoding service (e.g. Google Geocoding API).

  Geoparsing included the following features :
  - **token expansion** using location name variants (i.e. OSM multi-lingual names, short names and acronyms)
  - **token expansion** using location type variant88s (e.g. street, st.) 
  - **token filtering** of single token location names against WordNet (non-nouns), language specific stoplists and peoples first names (nltk.corpus.names.words()) to reduce false positive matches
  - **prefix checking** when matching in case a first name prefixes a location token(s) to avoid matching peoples full names as locations (e.g. Victoria Derbyshire != Derbyshire)

  **Location disambiguation** is based on an evidential approach, with evidential features detailed below in order of importance:
  - **token subsumption**, rejecting smaller phrases over larger ones (e.g. ‘New York’ will prefer [New York, USA] to [York, UK])
  - **nearby parent region**, preferring locations with a parent region also appearing within a semantic distance (e.g. ‘New York in USA’ will prefer [New York, USA] to [New York, BO, Sierra Leone])
  - **nearby locations**, preferring locations with closeby or overlapping locations within a semantic distance (e.g. ‘London St and Commercial Road’ will select from road name choices with the same name based on spatial proximity)
  - **nearby geotag**, preferring locations that are closeby or overlapping a geotag
  - **general before specific**, rejecting locations with a higher admin level (or no admin level at all) compared to locations with a lower admin level (e.g. ‘New York’ will prefer [New York, USA] to [New York, BO, Sierra Leone]

    [geoparsepy user documentation](https://pythonhosted.org/geoparsepy/readme.html)

    [geoparsepy API documentation](https://pythonhosted.org/geoparsepy/index.html)

    [Github Similar Example](https://github.com/buyuhuang/cliowire-bots)
  
### Articles

- [ ] [Geoparsing and Geosemantics for Social Media: Spatio-Temporal Grounding of Content Propagating Rumours to support Trust and Veracity Analysis during Breaking News](http://delivery.acm.org/10.1145/2850000/2842604/a16-middleton.pdf?ip=144.82.115.188&id=2842604&acc=ACTIVE%20SERVICE&key=BF07A2EE685417C5%2ED93309013A15C57B%2E4D4702B0C3E38B35%2E4D4702B0C3E38B35&__acm__=1528231885_048e3235cf7afab80aa9bd4326986742)
- [ ] [Real-Time Crisis Mapping of Natural Disasters Using Social Media](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=6692841)

## 2018-6-13

### Datasets

#### Twitter API

<https://developer.twitter.com/en/docs.html>


#### TfL Open Data

<https://tfl.gov.uk/info-for/open-data-users/our-open-data>
<https://api-portal.tfl.gov.uk/docs>
<https://blog.tfl.gov.uk/>

- [API](https://api.tfl.gov.uk/)
  - Stop Points
    - "CarPickupSetDownArea",
    - "NaptanAirAccessArea",
    - "NaptanAirEntrance",
    - "NaptanAirportBuilding",
    - "NaptanBusCoachStation",
    - "NaptanBusWayPoint",
    - "NaptanCoachAccessArea",
    - "NaptanCoachBay",
    - "NaptanCoachEntrance",
    - "NaptanCoachServiceCoverage",
    - "NaptanCoachVariableBay",
    - "NaptanFerryAccessArea",
    - "NaptanFerryBerth",
    - "NaptanFerryEntrance",
    - "NaptanFerryPort",
    - "NaptanFlexibleZone",
    - "NaptanHailAndRideSection",
    - "NaptanLiftCableCarAccessArea",
    - "NaptanLiftCableCarEntrance",
    - "NaptanLiftCableCarStop",
    - "NaptanLiftCableCarStopArea",
    - "NaptanMarkedPoint",
    - "NaptanMetroAccessArea",
    - "NaptanMetroEntrance",
    - "NaptanMetroPlatform",
    - "NaptanMetroStation",
    - "NaptanOnstreetBusCoachStopCluster",
    - "NaptanOnstreetBusCoachStopPair",
    - "NaptanPrivateBusCoachTram",
    - "NaptanPublicBusCoachTram",
    - "NaptanRailAccessArea",
    - "NaptanRailEntrance",
    - "NaptanRailPlatform",
    - "NaptanRailStation",
    - "NaptanSharedTaxi",
    - "NaptanTaxiRank",
    - "NaptanUnmarkedPoint",
    - "TransportInterchange"
  - NaptanToNlcMappings.json

- [Road Data](http://roads.data.tfl.gov.uk/)
  - Levels of traffic flow and delay  (17/12/2017-16/03/2018, Congestion SCOOT 15 minutes)  
  - Journey times on London’s main roads (4/2017- 4/2018, LCAP 5 minutes)
  - TrafficMaster: Average speeds on London’s main roads (2016-2017, Peak Periods & 4-week aggregation)

- [Oyster card data](http://data.tfl.gov.uk/tfl/syndication/feeds/oystercardjourneyinformation.zip?app_id=44a8c3d8&app_key=2ff35c20e63cba085e6f00ed5853ec40)

  Oyster card journey information
  This dataset provides a 5% sample of all Oyster card journeys performed in a week during November 2009 on bus, Tube, DLR and London Overground.

- [London Underground Stations Passenger Counts Data](tap.data.tfl.gov.uk)

#### Met Office

- [Met Office MOGREPS data](http://data.informaticslab.co.uk/mogreps_data_basics.html)

- API

- [Geovation: Britain's Location and Property Data Lab](https://geovation.uk/)

#### Ordnance Survey

<https://www.ordnancesurvey.co.uk/>

- Open Data()
- MAPs API
- [PLACEs API](https://developer.ordnancesurvey.co.uk/os-places-api)
- [NAMEs API](https://developer.ordnancesurvey.co.uk/os-names-api)
- ROUTEs API
- [Open Capacity](http://opencapacity.co/)

### Articles

#### Profiling people and places for targeted advertising

`-> Geolocated Tweets`

<https://www.ucl.ac.uk/spacetimelab/docs/SpaceTimeLabLeafletMay2016>

There are 24 million journeys made across London’s
transportation network per day. By profiling people
and the places they visit, SpaceTimeLab gains insights into needs, allowing businesses to target their advertising in the right places.

We use **geolocated Tweets** to understand what people
use different parts of the city for. Our research can help TfL to decide what advertising to place in their London Underground stations.

#### Modernising the National Travel Survey

`-> Geolocated Tweets`

<https://assets.publishing.service.gov.uk/government/uploads/system/uploads/attachment_data/file/641452/modernising-the-national-travel-survey.pdf>

### Blogs

#### Me, Geolocated on Twitter

`-> Geolocated Tweets`

<http://oobrien.com/2012/12/me-geolocated-on-twitter/>

### Python Packages

#### Tweepy

[Twitter数据挖掘：如何使用Python分析大数据](http://www.itran.cc/2017/06/15/twitter-data-mining-using-python/)

Twitter Data Mining: A Guide to Big Data Analytics Using Python

## 2018-6-14

### TODO

- [ ] Twitter API 抓取！
- [ ] Coursework Codes upload

## 2018-6-26

### TODO

- [ ] Twitter API

## 2018-07-04

### ogr2ogr

convert shp file to csv etc.

eg. `ogr2ogr -f "CSV" gis.osm_pois_free_1.csv gis.osm_pois_free_1.shp -lco GEOMETRY=AS_XY`

### geoparsepy

convert it from python 2 to python 3 using 2to3.script

[differences between python 2 and 3](https://www.zhihu.com/question/19698598)

[future package: Easy, clean, reliable Python 2/3 compatibility](http://python-future.org/compatible_idioms.html#strings-and-bytes)

### TODO

- [ ] type: str, byte...; encode, decode

- [ ] package: nlpk, [book](https://www.nltk.org/book/)