# Tweet Summarizer

## Overview

Takes data from a database of tweets from selected sources, then pre-processes them in order 
to run natural language processing tools in order to summarize them. This application has two notebooks,
with different methods to process tweets:

1. the Rule Based Summarizer
2. the Supervised Learning Summarizer

This application is designed to summarize _individual_ tweets and prepare them for further analysis for actual 
event extraction.

### The Rule Based Summarizer

This summarizer simply extracts parts of speech from tweet text using the spaCy NLP library's built-in 
models. 

### The Supervised Learning Summarizer (in progress)

This summarizer uses spaCy for initial text processing, but then uses machine learning techniques to extract 
further data from each tweet. 

*Requires More Data*

## Application Suite

This application is part of a testbed suite to take data from microblogs (in this case, Twitter) 
and extract event data from them. The end result of this (in progress) research project is to have an output 
of news-worthy event summaries that is generated in real-time as tweets are produced. As of now, 
this suite consists of the following applications:

* The Tweet Summarizer (_this application_)
* The Tweet Categorizer
    * Once individual tweets are summarized, this application will categorize tweets based on (TBD) criteria.
* The Event Visualizer
    * This will take event data and show it in a UI, with geolocation and tabular data viz. 