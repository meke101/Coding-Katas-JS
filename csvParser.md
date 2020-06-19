## CSV Parser

CSV files (comma separated values) are a very common format for exporting table structured data. The first line of the file represents the headers of each column and each consecutive line represents a row of data (columns separated by commas, rows separated by new line characters).

The goal of this kata is to implement your own CSV parser that takes in CSV string and returns an array of JavaScript objects with the corresponding key-value pairs.

We supply you with a sample CSV file in the `data` directory, but feel free to use any dataset you want.

You'll need to find a way to import the CSV file into your JS file as a string. **Hint:** Node.js has a built in module for reading and writing files.

##### examples

List examples of some passing tests

###### `data/cities.csv`
``` CSV
city,state,population,land area
seattle,WA,652405,83.9
new york,NY,8405837,302.6
boston,MA,645966,48.3
kansas city,MO,467007,315.0
```


```javascript
    xsvParser(csvString);
    // =>
    /*
    [
        {
            "city": 'seattle',
            "state": 'WA',
            "population": 652405,
            "land area": 83.9
        },
        {
            "city": 'new york',
            "state": 'NY',
            "population": 8405837,
            "land area": 302.6
        },
        ... etc.
    ]
    */
```
