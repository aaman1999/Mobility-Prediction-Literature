# Literature on human mobility modeling and prediction
In this repository you will find the metadata of all the relevant literature concerning human-mobility modeling and prediction.
The source codes for scrapping, cleaning and preprocessing this data.

## From where is this data collected?  
  - [Web of Science](https://apps.webofknowledge.com/WOS_GeneralSearch_input.do?product=WOS&search_mode=GeneralSearch&SID=C5uHbS2XkmFRw4V47rb&preferencesSaved=)
  - [Microsoft Academic Search](https://preview.academic.microsoft.com/home)
  - [Semantic Scholar](https://www.semanticscholar.org/)

## How is the scraping and crawling done?
- The scrapping from Semantic Scholar is done using [Semantic Scholar API](https://api.semanticscholar.org/).
- The [maka Python module](https://github.com/gfhuertac/maka) is used to scrape data from Microsoft Academic Search. W
- Web of Science permits to manually download data for selected topics under a university lisence.

## What key-words and domains were selected to scrape this data?
The scrapping was done using the following Keywords:
- Human-mobility prediction
- Human-mobility modeling
- Next place forecasting
- Next place prediction
- Predicting User Movement
- Predicting Significant locations
- Predicting User Movement

## and restricted to the following domains:
 - [Computer science, Computer network, Mobility model, Distributed computing, Real-time computing, Wireless ad hoc network]
 - [Handover, Artificial intelligence, Optimized Link State Routing Protocol, Machine learning, Quality of service]
 - [Wireless Routing Protocol, Data mining, KDD, Wireless network, Mobile ad hoc network, Ad hoc wireless distribution service]
 - [Mobile computing, Mobility management, Adaptive quality of service multi-hop routing]

## How does the pipeline for the collection and cleaning process look like?
![alt text](https://github.com/vaibhav90/Mobility-Prediction-Literature/blob/master/images/scrapping.png)

## How was the cleaning, duplicate removal and unrelated item removal was done?
- The string similarity and profiling was performed using [python-string-similarity](https://github.com/luozhouyang/python-string-similarity).
- The raw_data folder contains raw data scrapped from all the platforms with the title indicating the key word searched.
- The scripts folder contains python scripts used to scrape, preprocess, clean and merge the data collected from different sources.
- The file literature_metadata contains the merged list and literature_with_abstracts contains all the abstracts.

## What is the format of the data?
Paper Title | Publication Year | Publication Venue | Authors | Keyword List
![alt text](https://github.com/vaibhav90/Mobility-Prediction-Literature/blob/master/images/met_data.jpg)
