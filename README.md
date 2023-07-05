# county_research


Use:
```
source county/bin/activate 
```

to activate virtual env


ReduceRedfinData.ipynb takes the raw `county_market_tracker` and turns it into something more manageable. It deletes unnecessary columns and unnecessary years.

It spits out `data/redfin_county_data_2023-05.xslx`.

Then AverageRedfinData.ipynb takes that averages the values on a one month, 3 month, 6 month horizon.
Its output file is: `processed/redfin_month_rollup_2023-05.xslx` 

Then CombineDate,pyn merges it


## Updating Base Data:

```
Download data from:
https://redfin-public-data.s3.us-west-2.amazonaws.com/redfin_market_tracker/county_market_tracker.tsv000.gz
```

