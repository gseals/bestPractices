React begins
invented by FB in 2013
most jobs in Nashville are React or Angular

react acts in the way that you are building out components that you can reuse (like the card we've built); we are doing a lot less writing of UI components and 
breaking down the application into small bits and injecting into other projects/locations

jsx is writing html in JS

all of the create react app happens on master; the setup branch will be for what Zoe wants us to change and do

do not initialize with a readme in github

react process:
npx create-react-app intro-react


git remote -v to see the connections to github

delete app.test.js
create folder called App and move 2 apps and logo
change import statements in index.js
package.json remove test from scripts
* create folder called Styles and move index.css into the folder
* rename index.css to index.scss
* index.js and change imports
* delete setuptest.js
* rename app.css to app.scss
* install node-sass

npm install eslint-config-airbnb-base --save

CANNOT use the word class in jsx because it is a reserved word; must use className

git rm package-lock.json --cache then git status

# **Begin here**:

be sure you are in the folder you want this directory to live
in your terminal: npx create-react-app 'name of your directory'
example: if the name of your directory is 'starting', then npx create-react-app starting

in github, create repo of the same name but do not initiliaze with a readme

terminal: cd into directory you just made

*copy github line into terminal (the 'git remote add origin' line)

terminal: git rm package-lock.json --cache

*open code in vscode and gitignore package-lock.json

git add .

git commit

git push -u origin master

git checkout -b 'setup branch'



delete app.test.js and setuptest

delete test line from package.json

create new folders: App and styles in src

move app.js and app.css and logo.svg into App folder

update app.css to app.scss

index.css goes to styles

update index.css to index.scss

install lintr:
npm install eslint-config-airbnb-base --save-dev

create .eslintrc and copy things from [instructions](https://github.com/nss-nightclass-projects/Night-Class-Resources/blob/react/book-4-react/chapters/react-setup.md#add-eslint) to be linted into it

index.scss: add .App background color line

in styles, create _variables.scss, add a color variable, import into index.scss

install node sass
npm install node-sass --save

index.js : change the import path for index.css and App

App.scss remove background-color

install bootstrap/firebase/axios
npm install axios bootstrap firebase jquery popper.js --save

put your test button App.js

App.js correct App.css import statement

top of index.scss:
@import '~bootstrap/dist/css/bootstrap.min.css';

npm install prop-types --save
