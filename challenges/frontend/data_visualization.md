# Simple data processing app

**Using this simple data set**

```javascript
revenue = [
  { date: "2015-01-01", value: 14 }
  { date: "2015-01-02", value: 21 }
  { date: "2015-01-03", value: 31 }
  { date: "2015-01-04", value: 16 }
  { date: "2015-01-05", value: 18 }
  { date: "2015-01-08", value: 29 }
  { date: "2015-01-09", value: 36 }
  { date: "2015-01-10", value: 42 }
  { date: "2015-01-11", value: 33 }
]

costs = [
  { date: "2015-01-01", value: 7 }
  { date: "2015-01-02", value: 11 }
  { date: "2015-01-03", value: 14 }
  { date: "2015-01-04", value: 10 }
  { date: "2015-01-05", value: 8 }
  { date: "2015-01-06", value: 15 }
  { date: "2015-01-07", value: 16 }
  { date: "2015-01-10", value: 19 }
  { date: "2015-01-11", value: 16 }
]

```

**build a small app with backbone, angular or react that**
- joins the two datasets into one
- adds an additional computed "profit" (= revenue - costs) to the dataset
- has one "page" showing a table with the data (ideally sortable by any column)
- has one "page" displaying a line chart with the data (ideally using d3)
- has some test coverage
