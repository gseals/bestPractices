## Class

### October 26, 2019

### JSON

* what gets returned when you hit an API
* cannot comment JSON files
* JS object with quotes around the keys
* [json lint](https://jsonlint.com/) - a web resource to ensure your JSON is a valid JSON file
* validate your json every single time; it will save you a ton of time later
* JS with extra quotes everywhere; has to be double quotes
* firebase is an object storge database which means it doesn't understand arrays
* to upload to firebase, upload an object of objects
* when we pull the code in, we have to make it an array of objects

### ERD

* Entity relationshiop diagrams
* used when doing architecture for a new API
* you always need some kind of agreement on what's going into your database when you make a database
* map out all the relationships between the diff types of tables I'm going to need, what are the data types in those, and what are the realtioship between all of those
* ids are important to the relationships because they are unique
* when you send for data to firebase, firebase will create an id for you
* firebase calls objects of objects (or tables), collections
* if you have repetitive information, look for ways to simplify
* we do not want arrays inside of any collection
* [lucid chart](https://www.lucidchart.com/pages/) - charting tool for ERDs, flow charts, anything you need to graph
  * horizontal line stands for one relationship, the forked end stands for many
* team treehouse: by adding .json to the end of the url, you can access the json data
  * only available on websites that expose their api

### Axios

* axios returns Promises (more to come on October 28)
* [axios](https://github.com/axios/axios) github