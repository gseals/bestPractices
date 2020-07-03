## Deploy on Github

#### package.json

* beneath "private": true and above "dependencies":, add this line:

* "homepage": "https://gseals.github.io/React-Movie-Database/"

* replace React-Movie-Database with the appropriate name for your repo/project

#### package.json

* in "scripts", between "start" and "build", place these two lines:

* "predeploy": "npm run build",
* "deploy": "gh-pages -d build",

#### Terminal

* run this line of code and change React-Face-Detect to reflect the actual GitHub url of your project:

* git remote set-url origin https://github.com/gseals/React-Face-Detect

#### Terminal

* Run these lines of code:

* npm install gh-pages --save-dev

* npm run build

* npm run deploy