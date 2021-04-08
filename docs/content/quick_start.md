# Quick Start Guide

## Getting Started
If you'd like to access the CPN data, please [visit our website](https://www.barchart.com/cmdty/data/pricing-network) and fill out the "Get Started" form. You can also send us an email at cmdty@barchart.com. Should you have suggestions on what to included, please let us know. It's worth nothing that the more information you can provide us in the request will allow us to deliver a solution which best fits your needs. Some information that would be helpful would include:
* Use Case - What are you looking to do with the information?
* Data Access - Is your application public or only available to subscribers?  Can users download the data?
* Historical Data - Do you require historical information or only current prices?

Once we have an understanding of what you're looking to do our team will be able to get you started.


## Making Your First Query

As an example, let's retrieve quotes for the symbols you are interested in: 
* Open your favorite web browser
* Enter you API key and symbols into the url template: http://ondemand.websol.barchart.com/getQuote.json?apikey=YOUR_API_KEY&symbols={SYMBOLS_INTERESTED_IN} 
* Copy and paste the url into the browser, and hit enter
* Voila! The API will return latest data for the symbols to your browser, similar to below:
```
{
  "status": {
    "code": 200,
    "message": "Success."
  },
  "results": Array[2][
    {
      "symbol": "MTC031V.CP",
      "name": "Beef cutout choice whs C US",
      "dayCode": "1",
      "serverTimestamp": "2021-04-01T11:51:08-05:00",
      "mode": "i",
      "lastPrice": 2.36,
      "tradeTimestamp": "2021-04-01T00:30:17-05:00",
      "netChange": 0,
      "percentChange": 0,
      "unitCode": "2",
      "open": 2.36,
      "high": 2.36,
      "low": 2.36,
      "close": null,
      "numTrades": 1,
      "dollarVolume": 0,
      "flag": "",
      "volume": 0,
      "previousVolume": 0
    },
    {
      "symbol": "MTC031W.CP",
      "name": "Beef cutout select whs C US",
      "dayCode": "1",
      "serverTimestamp": "2021-04-01T13:22:57-05:00",
      "mode": "i",
      "lastPrice": 2.24,
      "tradeTimestamp": "2021-04-01T00:30:17-05:00",
      "netChange": 0,
      "percentChange": 0,
      "unitCode": "2",
      "open": 2.24,
      "high": 2.24,
      "low": 2.24,
      "close": null,
      "numTrades": 1,
      "dollarVolume": 0,
      "flag": "",
      "volume": 0,
      "previousVolume": 0
    }
  ]
}
```

## Explore More

Congrats! You've made your first query. Feel free to check more details about our [onDemand](https://www.barchart.com/cmdty/data/ondemand) APIs. Here you can explore more advanced methods of querying CPN data.
