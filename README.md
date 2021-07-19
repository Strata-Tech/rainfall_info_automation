# Rainfall Info Automation for insurance companies


## Background
Insurance company offer protection against surge pricing on ride hailing companies (i.e Grab, Gojek,Ryde). Example of such insurance coverage provided is Droplets. https://www.droplet.sg/#/ . Such a plan protects commuters against unpredictable surge pricing on ride-hailing platforms when it rains.

Surge pricing, the practice of hiking up ride-hailing fares in times of high demand, usually kicks in when it rains.Surge pricing occurs when the demand for drivers suddenly increases like during bad weather or due to rush hour. To ascertain the amount of rainfall we can reference the amount of rainfall at a given time.

There are 60 weather stations in Singapore which measures rainfall, and utilizing data from MSS (Meteorological Service Singapore) and calling a public API we can get real time feeds of rainfall at various locations


![Screenshot 2021-07-19 at 1 45 42 PM](https://user-images.githubusercontent.com/77420780/126109182-9d826bd6-7c71-43ec-b5c6-d6b02b685043.png)

Source:data.gov.sg

To see the number of catchment areas pls refer to : https://data.gov.sg/dataset/realtime-weather-readings/resource/8bd37e06-cdd7-4ca4-9ad8-5754eb70a33d/view/b91b76be-21be-4cd4-b815-e2cc277475d7

## API Used
[Rainfall across Singapore API](https://data.gov.sg/dataset/realtime-weather-readings?resource_id=8bd37e06-cdd7-4ca4-9ad8-5754eb70a33d) - No API Key needed, but see [Singapore Open Data License](https://data.gov.sg/open-data-licence) which has further information on its usage.

To aid insurance companies monitor whether claims are valid, or to do dynamic pricing, we will want to know whether is it raining now (0mm - no rainfall, >0mm - rainfall) and how heavy the rainfall is at various locations.

How high will the surge pricing be (the heavier the rainfall, the higher the surge pricing)
In this project I automated the rainfall feeds which can further aid insurance companies to automate their pricing strategy.

## Technologies used
Requests

## Data Preprocessing 
From the calling the API ,I cleansed the JSON file to get the various stations in Singapore and rainfall feed when it rains in a key-value dictionary pair.

## Desired Outcome
From the app , we are able to get automated info on the amount of rainfall at a particular area. With this info insurance companies can validate the claims of their clients as well as set dynamic pricing for such insurance plans.
