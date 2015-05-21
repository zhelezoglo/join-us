# Combine datasets

First unzip the data in `spark/` (both gzip and zip formats are provided)<sup>1</sup>.

#### Output required:
List the top 5 countries by 'Electricity production (kWh)' in 2005, plus print the additional properties for each country: 'Long Name' & 'Region'.

Ignore any countries that do not have a 'Region' code, e.g. 'World'.

Sample output:
```
1. Andora: 5500 (Principality of Andora, Europe & Central Asia)
2. Congo: 3400 (Republic of Congo, Sub-Saharan Africa)
3. ...
4. ...
5. ...
```

#### Notes: 
* Use data frames (`createDataFrame`) using the csv header rows as the data frame column list
* Assume basic csv parsing - it's enough to split each line on a pipe `|` symbol to get the cells
* data.csv should be joined to countries.csv using 'Country Code'
* Try and let the spark nodes do as much of the work as possible - e.g. don't call collect() on the full set of data.

<sup>1</sup> The data is taken from the World Bank development indicators website (http://databank.worldbank.org/).
Some small modifications were made to make this task more about data transformation, less about csv cleanup.

