[![Build Status](https://api.travis-ci.org/jasper07/saptech15.svg?style=flat)](https://travis-ci.org/jasper07/saptech15)
# SAPTech15 - Supercharge Your UI5 Developments By Adding Some Grunt

**The objective of the presentation**

Highlight to audience that to do SAPUI5 properly you have to go beyond the tutorials and set up tasks and process to manage team, build and deploy etc.

**The target audience**

Architects, Developers and Mangers thinking about or doing SAPUI5 developments.

**The problem** 

New paradigm, team will have limited experience, limited time to learn

**the solution**

a workflow for you UI5 development with Gruntjs, covering develop, analyse, test, build and deploy

**Presentation slides**

http://jasper07.secondphase.com.au/presentation-saptech15/


## Install Node
[https://nodejs.org/](https://nodejs.org/)

Open terminal and install Grunt and Bower

```javascript
npm install -g grunt-cli bower
```

## Installing the application

```javascript
git clone https://github.com/jasper07/saptech15.git
npm install
bower install
```

## Run the app
```javascript
grunt serve
```

this will setup a server which hosts the app, open up your browser and point it to

[http://localhost:8080/index.html](http://localhost:8080/index.html)

This will take you to the index page, from here you can

##  Start the app with mock data

[http://localhost:8080/testService.html](http://localhost:8080/testService.html)

## Start the app with optimized code
[http://localhost:8080/build.html](http://localhost:8080/build.html)

## To run the Unit and Opa tests in the browser

[http://localhost:8080/test/unit/unitTests.qunit.html](http://localhost:8080/test/unit/unitTests.qunit.html)

[http://localhost:8080/test/integration/opaTests.qunit.html](http://localhost:8080/test/integration/opaTests.qunit.html)


## Build the code
Clean: clean the "dist" directory
Openui5_Preload: Optimize the code by concatenating and minifying soure into a sinle preload component
Copy: Copy new source to "dist" directory
Replace: Replace banner on all files

```javascript
grunt build
```

## Analyze the code
Run Eslint accross the code base to check for syntax and formatting errors

```javascript
grunt lint
```

## Test the code running in a headerless browser
use one of the following commands to run both, or run individual
```javascript
grunt test

grunt unitTest

grunt opaTest
```

## To integrate with Travis-CI
A CI tool makes working in a team easier with automated builds. These builds are triggered automatically when each developer checks in their code to the repository. The build process incorporates testing, if testing fails the build stops and team members will be notified.

#### how to, very quick only a couple of steps
[http://code.tutsplus.com/tutorials/travis-ci-what-why-how--net-34771](http://code.tutsplus.com/tutorials/travis-ci-what-why-how--net-34771)

the results
[https://travis-ci.org/jasper07/saptech15](https://travis-ci.org/jasper07/saptech15)




