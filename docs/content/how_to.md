# How To
In this section we provide you with details of how you can interact with CPN data.  Should you have suggestions on what to include, please let us know.

## Get latest data in cmdtyView

You can access all the CPN data in our platform [cmdtyView](https://www.barchart.com/cmdty/trading/cmdtyview) using your web browser or mobile. Access the latest quotes, historical data and create visualization to analyze trends and generate insights. 

* **Get Started** - Go to our [website](https://www.barchart.com/cmdty/trading/cmdtyview), click on the "Get Started" button to connect with our team and get access to cmdtyView
* **Creating Workspace** - Explore how to [create a fully-customizable Workspace](https://www.barchart.com/cmdty/video/cmdtyview-creating-workspace) within cmdtyView.
* **Collaborate with your Team** - Explore how to easily [share a Workspace](https://www.barchart.com/cmdty/video/cmdtyview-sharing-workspace) within cmdtyView to present your workspace and analysis to you team.

## Get data delivered in Excel

If Excel is your go to tool for analysis, we have got you covered. Get the data delivered directly into Excel via [cmdtyView Excel](https://www.barchart.com/cmdty/trading/cmdtyview-excel) to take your research to the next level.

* **Download** - [Click here to download](https://install.barchart.com/cmdty-excel/setup.exe) the cmdtyView Excel Add-in to get started.
* **Quick Start Guide** - From installation through to getting your first quote live in Excel, our [quick start guide](https://barchartsolutions.atlassian.net/wiki/spaces/CUG/pages/391053370/Getting+Started) will have you building amazing workbooks in no-time. Drop at line at real-time@barchart.com if you have any questions.
* **Template Gallery** - Take a look at [our gallery of templates](https://barchartsolutions.atlassian.net/wiki/spaces/CUG/pages/393740347/Excel+Templates) for a multitude of use cases. Get started faster with pre-built tools that have been battle tested by our team of analysts and designed from the feedback of our users.


## Enterprise Solutions

Get the commodity prices you need, when you need it - and delivered today. Our APIs for commodity data are fast, flexible, and available OnDemand.

### Get Quotes
Get the latest data using our [getQuote](https://www.barchart.com/ondemand/api/getQuote) API.

http://ondemand.websol.barchart.com/getQuote.json?apikey=YOUR_API_KEY&symbols=MTC031V.CP,MTC031W.CP

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
### Get Historical Data
Get the historical data using our [getHistory](https://www.barchart.com/ondemand/api/getHistory) API.

http://ondemand.websol.barchart.com/getHistory.json?apikey=YOUR_API_KEY&symbol=MTC031V.CP&type=daily&startDate=20200101&endDate=20211201&order=desc

```
{
  "status": {
    "code": 200,
    "message": "Success."
  },
  "results": Array[325][
    {
      "symbol": "MTC031V.CP",
      "timestamp": "2021-04-01T00:00:00-04:00",
      "tradingDay": "2021-04-01",
      "open": 2.37,
      "high": 2.37,
      "low": 2.37,
      "close": 2.37,
      "volume": 0,
      "openInterest": null
    },
    {
      "symbol": "MTC031V.CP",
      "timestamp": "2021-03-30T00:00:00-04:00",
      "tradingDay": "2021-03-30",
      "open": 2.37,
      "high": 2.37,
      "low": 2.37,
      "close": 2.37,
      "volume": 0,
      "openInterest": null
    },
    .
    .
    .

}
```
