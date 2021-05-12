# Quick Start Guide

## Getting Started
If you'd like to access the cmdtyStats data, please [visit our website](https://www.barchart.com/cmdty/data/stats) and fill out the "Get Started" form. You can also send us an email at cmdty@barchart.com. Should you have suggestions on what to included, please let us know. It's worth nothing that the more information you can provide us in the request will allow us to deliver a solution which best fits your needs. Some information that would be helpful would include:
* Use Case - What are you looking to do with the information?
* Data Access - Is your application public or only available to subscribers?  Can users download the data?
* Historical Data - Do you require historical information or only current prices?

Once we have an understanding of what you're looking to do our team will be able to get you started.


## Making Your First Query

As an example, let's retrieve data for the symbols you are interested in: 
* Open your favorite web browser
* Enter you API key and symbols into the url template: https://ondemand.websol.barchart.com/getCmdtyStats.json?apikey=YOUR_API_KEY&symbol=USDA-SOYB-PROD-MS-96.CS&startDate=20200512&endDate=20210512&order=asc 
* Copy and paste the url into the browser, and hit enter
* Voila! The API will return latest data for the symbols to your browser, similar to below:
```
{
    "status": {
        "code": 200,
        "message": "Success."
    },
    "results": [
        {
            "symbol": "USDA-SOYB-PROD-MS-96.CS",
            "shortSymbol": "UD09002O.CS",
            "shortName": "MS Soybeans PROD",
            "mediumName": "MS Soybeans PROD",
            "longName": "MS Soybeans Production",
            "seriesDescription": "Soybeans;Production,Annual,Bushel;Mississippi;Soybeans for Beans Area Harvested, Yield, and Production",
            "item": "Soybeans",
            "measurement": "Production",
            "frequency": "Annual",
            "unit": "Bushel",
            "multiplier": 1,
            "area": "Mississippi",
            "areaType": "State",
            "sources": [
                "USDA",
                "NASS",
                "Crop Production",
                "Soybeans for Beans Area Harvested, Yield, and Production",
                "NASS Crops"
            ],
            "unitDescription": "Bushel",
            "lastRefresh": "2020-11-10",
            "stats": [
                {
                    "date": "2020-12-31",
                    "value": "111240000"
                }
            ]
        }
    ]
} 
```

## Explore More

Congrats! You've made your first query. Feel free to check more details about our [onDemand](https://www.barchart.com/cmdty/data/ondemand) APIs. Here you can explore more advanced methods of querying cmdtyStats data.
