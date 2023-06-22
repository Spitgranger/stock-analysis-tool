# Stock analysis tool
Pulls data from Yahoo Finance then provides functions to analyze stocks.
Currently generates a spreadsheet with indicators, five day performance, ten day performance, twenty day performance, can apply conditional formatting to help filter
## Functions
### `get_data(symbols, time_period)`
This function returns a pandas dataframe containing the historical closing prices of the ticker symbols passed to it.
| Parameters | Description |
| ---------- | ----------- |
| symbols | a list of all desired symbols, in the same format as Yahoo Finance |
| time_period | a string of the desired period of data ex. "1y", "2y" .. |

### `filter_five_days(df)`
This function returns a pandas dataframe containing the five day performance of the each of the stocks within the pandas dataframe passed to it.
| Parameters | Description |
| ---------- | ----------- |
| df | a pandas dataframe containing historical stock data. Should be the one returned by `get_data` |

### `filter_ten_days(df)`
This function returns a pandas dataframe containing the ten day performance of the each of the stocks within the pandas dataframe passed to it.
| Parameters | Description |
| ---------- | ----------- |
| df | a pandas dataframe containing historical stock data. Should be the one returned by `get_data` |

### `filter_twenty_days(df)`
This function returns a pandas dataframe containing the twenty day performance of the each of the stocks within the pandas dataframe passed to it.
| Parameters | Description |
| ---------- | ----------- |
| df | a pandas dataframe containing historical stock data. Should be the one returned by `get_data` |

### `filter_year(df)`
This function returns a pandas dataframe containing the 365 day performance of the each of the stocks within the pandas dataframe passed to it.
| Parameters | Description |
| ---------- | ----------- |
| df | a pandas dataframe containing historical stock data. Should be the one returned by `get_data` |


Total return is spreadsheet, to change modify the given ticker symbols
Note: Ticker symbols do not automaticaly update.
