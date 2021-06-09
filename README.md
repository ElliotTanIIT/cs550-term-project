# cs550-term-project

## Exploring the functional computational and capabilities of InfluxDB and TimescaleDB

The goal of this project was to compare two time series databases: InfluxDB and TimescaleDB. We compared both their functionality and computational capabilities. In order to measure their computational capabilities, we used Time Series Benchmark Suite (TSBS) and ran similar experments on the respective Time Series Databases.

InfluxDB is written in the GoLang while TimescaleDB is an extension of PostgreSQL, and both are time series databases.

### Functionality
Through thorough research, we learned that InfluxDB has a large advantage in its functional capabilities due to the various packages that it contains. Although there is a steeper learning curve to using InfluxDB because of it's custom SQL-like query language, users will find that it more flexible than TimescaleDB. Some of the packages allow it to store and retireve data as json, csv, or even Http protocols. InfluxDB also has a GUI with drop down menus to help build queries, allowing newer users to familiarize themselves with InfluxDBs system. In contrast, we found TimescaleDB to lack many of the functionalities that InfluxDB offered.

### Computational Capablity
After running TSBS, we found InfluxDB to have much faster single host query execution than TimescaleDB. This means that when only 1 user is accessing the database, InfluxDB outperforms TimescaleDB. However, when we ran the tests for multiple hosts and last point retrieval (getting the most recent record from database), we found that TimescaleDB worked faster.

### Which is Better?
In the case of data analysis, we would recommend InfluxDB for its numerous packages and flexibility in manipulating data, and its faster single host query speed. However, if a company wanted to have a storage database servicing multiple users, we would recomment TimescaleDB as it's query execution scales better with more people.

### Tools used

Time Series Benchmark Suite (TSBS), AWS linux VM, INfluxDB, TimescaleDB
