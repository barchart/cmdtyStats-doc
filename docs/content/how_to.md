# How To
In this section we provide you with details of how you can interact with cmdtyStats data.  Should you have suggestions on what to include, please let us know.

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

### Get cmdtyStats ID
Search for data series based on search parameters covering content, source, area, frequency, and more using our [getCmdtyStatsId](https://www.barchart.com/ondemand/api/getCmdtyStatsId) API.

https://ondemand.websol.barchart.com/getCmdtyStatsId.json?apikey=YOUR_API_KEY&commodity=Corn&measurement=Production&area=United+States+of+America&source=USDA&maxRecords=50&page=1

```
{
    "status": {
        "code": 200,
        "message": "Success."
    },
    "results": [
        {
            "shortSymbol": "UD04006I.CS",
            "seriesDescription": "Corn;Production,Annual,Bushel;Alabama;Corn for Grain Area Harvested, Yield, and Production"
        },
        {
            "shortSymbol": "UD04006J.CS",
            "seriesDescription": "Corn;Production,Annual,Bushel;Arizona;Corn for Grain Area Harvested, Yield, and Production"
        },
        {
            "shortSymbol": "UD04006K.CS",
            "seriesDescription": "Corn;Production,Annual,Bushel;Arkansas;Corn for Grain Area Harvested, Yield, and Production"
        },
        {
            "shortSymbol": "UD04006L.CS",
            "seriesDescription": "Corn;Production,Annual,Bushel;California;Corn for Grain Area Harvested, Yield, and Production"
        },
        {
            "shortSymbol": "UD04006M.CS",
            "seriesDescription": "Corn;Production,Annual,Bushel;Colorado;Corn for Grain Area Harvested, Yield, and Production"
        },
  .
  .
  .
 
}
```
### Get Historical Data
Get the historical data using our [getCmdtyStats](https://www.barchart.com/ondemand/api/getCmdtyStats) API.

https://ondemand.websol.barchart.com/getCmdtyStats.json?apikey=YOUR_API_KEY&symbol=USDA-SOYB-PROD-MS-96.CS&startDate=20200513&endDate=20210513&order=asc

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
