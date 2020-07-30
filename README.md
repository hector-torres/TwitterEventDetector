Twitter Event Detector
===
## Overview
The Twitter Event Collector is an application that automatically ingests tweets from 
selected sources, filters them for newsworthiness, extracts newsworthy features from them, 
categories news events from these features, then shares this data via a dashboard and API. 

### How It Works
The Twitter Event Detector contains the following jobs, each correalting with a s specific 
part of the event detection process. 

#### The Tweet Collector
Automatically ingests tweets and saves them to persistent storage.
#### The Newsworthiness Filter
Compares extracted tweet features against a corpus of headlines, verified news tweets, 
etc., using machine learning tools to detect newsworthy “events”
#### The Feature Extractor
Uses extracted features in order to try to categorize tweets based on a select number 
of news categories, with varying levels of importance assigned to each category. 
#### The Event Dashboard
Shows detected events in a UI that allows the user to select, filter, and parse events by 
location, time, or event type. 