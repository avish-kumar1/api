# COVID19-India API

A volunteer-driven, crowd-sourced database for COVID-19 stats & patient tracing in India.

[Source Code on Github](https://github.com/avish-kumar1/api)

## API Documentation

Detailed documentation regarding the API end-points [can be found here](documentation/)

### JSON Endpoints

| Status        | Data                                                                         | URL                                                     |
| ------------- | ---------------------------------------------------------------------------- | ------------------------------------------------------- |
| :green_heart: | Patient Level : Raw Data Partition 1 (Till Apr 19)                           | <https://avish-kumar1.github.io/api/raw_data1.json>           |
| :green_heart: | Patient Level : Raw Data Partition 2 (From Apr 20 to Apr 26)                 | <https://avish-kumar1.github.io/api/raw_data2.json>           |
| :green_heart: | Patient Level : Raw Data Partition 3 (From Apr 27 to May 09)                 | <https://avish-kumar1.github.io/api/raw_data3.json>           |
| :green_heart: | Patient Level : Raw Data Partition 4 (From May 10 to May 23)                 | <https://avish-kumar1.github.io/api/raw_data4.json>           |
| :green_heart: | Patient Level : Raw Data Partition 5 (From May 24 to Jun 04)                 | <https://avish-kumar1.github.io/api/raw_data5.json>           |
| :green_heart: | Patient Level : Raw Data Partition 6 (From Jun 05 to Jun 19)                 | <https://avish-kumar1.github.io/api/raw_data6.json>           |
| :green_heart: | Patient Level : Raw Data Partition 7 (From Jun 20 to Jun 30)                 | <https://avish-kumar1.github.io/api/raw_data7.json>           |
| :green_heart: | Patient Level : Raw Data Partition 8 (From Jul 01 to Jul 07)                 | <https://avish-kumar1.github.io/api/raw_data8.json>           |
| :green_heart: | Patient Level : Raw Data Partition 9 (From Jul 08 to Jul 13)                 | <https://avish-kumar1.github.io/api/raw_data9.json>           |
| :green_heart: | Patient Level : Raw Data Partition 10 (From Jul 14 to Jul 17)                | <https://avish-kumar1.github.io/api/raw_data10.json>          |
| :green_heart: | Patient Level : Raw Data Partition 11 (From Jul 18 to Jul 22)                | <https://avish-kumar1.github.io/api/raw_data11.json>          |
| :green_heart: | Patient Level : Raw Data Partition 12 (From Jul 23 to Aug 06)                | <https://avish-kumar1.github.io/api/raw_data12.json>          |
| :green_heart: | Patient Level : Raw Data Partition 13 (From Aug 07 to Aug 21)                  | <https://avish-kumar1.github.io/api/raw_data13.json>          |
| :green_heart: | Patient Level : Raw Data Partition 14 (From Aug 22 onward)                  | <https://avish-kumar1.github.io/api/raw_data14.json>          |
| :green_heart: | National Level :Time series, State-wise stats and Test counts                | <https://avish-kumar1.github.io/api/data.json>                |
| :green_heart: | State Level : has district-wise info                                         | <https://avish-kumar1.github.io/api/state_district_wise.json> |
| :green_heart: | State Level : Daily changes                                                  | <https://avish-kumar1.github.io/api/states_daily.json>        |
| :green_heart: | State Level : Testing data                                                   | <https://avish-kumar1.github.io/api/state_test_data.json>     |
| :green_heart: | National/State/District Level : Latest cumulative/daily counts               | <https://avish-kumar1.github.io/api/v4/data.json>             |
| :green_heart: | National/State/District Level : Specific date cummulative/daily counts       | <https://avish-kumar1.github.io/api/v4/data-YYYY-MM-DD.json>  |
| :green_heart: | National/State/District Level : Historical date-wise cumulative/daily counts | <https://avish-kumar1.github.io/api/v4/data-all.json>         |
| :green_heart: | National/State Level: Timeseries_(different structure)_                      | <https://avish-kumar1.github.io/api/v4/timeseries.json>       |
| :end:         | District Level : Daily changes                                               | <https://avish-kumar1.github.io/api/districts_daily.json>     |


### CSV

Sometimes, having files in a spreadsheet format is more useful for analysts and scientists. We have provided the files as downloadable csv files at the following location.

| Data                 | URL                                               |
| -------------------- | ------------------------------------------------- |
| Google sheets in CSV | <https://avish-kumar1.github.io/api/documentation/csv/> |

> :rocket: Quick example : Apply the formula `=IMPORTDATA("https://avish-kumar1.github.io/api/csv/latest/state_wise.csv")` in A1 cell of a Google Sheets to get the state data for analysis :)

## How this works

- Data in this repository is generated from Google Sheets
- Volunteers collect data from trusted sources and update the sheet
- Github Actions periodically fetch the data from the sheet and upload static json and csv files into `gh-pages` branch of this repo
- `gh-pages` serves the json/csv files at <https://avish-kumar1.github.io/api>

## License

This repository contains both the code that routinely fetches the data from Google Sheet and convert it into JSON files in the required format and the data itself (in the gh-pages branch). So, the content of this repository is licensed in two ways : Code and Data

License for Code (Consider this as everything in the `master` branch) : MIT License (Detailed in LICENSE_CODE.txt)  
License for Data (Consider this as everything in the `gh-pages` branch) : CC-BY-SA-4.0 License (Detailed in LICENSE_DATA.txt)

............................................
