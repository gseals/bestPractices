### October 28, 2019 - Promises and Asynchronous JS

* .data returns the whole file; without that, you get a promise

* use object.keys to return the names of the keys
* Object.keys returns an array; we can then use a forEach 
* .id assigns an id key to the object
* arrays have methods so changing the object to an array
* use objects when you're on an individual thing and you want to display it
* objects don't care about the key-value order
* array methods allow you to do more


#### Promises

synchoroous means that if you have a file, that file is read from top to bottom. JS is synchrnous
this is great until you need to make requests that take some time

every time the code is able to move on without a result, it's just going to return undefined

event listeners are what we do when we wait for something. these are called callback functions

with an xhrhttp, you define a success event listener and a failed event listener

pyramid of doom or callback hell - very difficult to tell what function is dealing with what

.then and .catch; .then can be chained together

promises are callbacks. it takes all of the requests for you

promises allow you to handle the way that the response comes back

axios makes an http request, a get request

the get request returns a promise so that you can handle what comes back from the get request

most browsers have a timeout code; you should not write a timeout

with a promise, you are saying who cares when you come back, I know how I'm going to handle you when you return

axios vs promise; axios makes the http request; promise is the machanism to access that information

to delete from firebase, use an axios.delete

promises recognize the promise call and allow your code to keep running

constructors: date, 

const firstPromise = new Promise((resolve, reject) => {
  const data = getInfo();
  if (data !== null) {
    resolve(data)
  } else {
    reject('Erorr, could not get data!');
  }
});

newPromise.then((resolvedData) => {
  printToDom(resolvedData)
})

  resolve(someValue);
  reject("failure reason");
});

promises are a new pattern you need to recognize

const getCows = () => new Promise((resolve, reject) => {
  axios.get('../../../../db/cows.json').then().catch();
});
this is a promise in a promise 

promises are pattern recognition

we always want the results to be an array of objects;

when you need to modify the data first, wrap it in a promise

don't work with XML

we will use these promises in the same way for the next year

if you are gonna modify the data, you need to wrap the axios promise in your own promise; if you are going to use the data just as it comes, you just need an axios call

it's good to have a unique identifier for when we need to modify the data
demFarmerCows[demFarmerCowId].id = demFarmerCowId;
this line assigns a unique identifier

spread operator start with an object and spread out of all the key:value pairs in the object; think of it as a copy; makes a copy of cow that is never able to be rferenced as the original cow