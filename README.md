# js-dev-env
JavaScript Development Environment from Pluralsight Course

VS Code/Atom/WebStorm
editorconfig.org

npm
package.json

js vulnabirities check
retire.js
nsp (nodesecurityplatform)

development webservers
http-server
lightweight (Support live-reloading)
express (not only for static files, can be used in production) (koa;hapi - alternatives)
budo (browserfy)
webpack (if chosed as bundler)
browsersync (anyones content is synchronized)

share work
localtunnel - hosts locally 
ngrok - hosts locally, adds security auth token
surge
now

Automation
Grunt (File oriented)
Gulp (Memory oriented)
npm Scripts

Transpilers
Babel - latest to ES5
TypeScript - TypeSafe
elm? - functional

Bundlers

ES6 - future
Browserify - the first, vast plugin base, simple
WebPack - established, versatile
RollUp - treeshaking +++
JSPM - 

experiment with sourcemap settings

linter

ES Lint
	Configuration file format?
	Which Rules
	Warning or Errors
	Plugins for specific style github awesome eslint
	start with preset (recomended, or airbnb; xo; standard JS)

npm eslint-watch for file watching

Testing /integration

	Framework
		+ Mocha - popular, does not include assertion library
		Jasmine - popular, assertion lib built in
		tape - leanest
		qunit
		ava
		jest - popular for react, nice wrapper for jasmine, facebook could be future
	Assertion Library - declare what you expect
		+chai - popular
		should.js
		expect
	Helper library 
		+jsdom - run tests without browser
		cheerio - jquery for the server, query dom using selectors
	where to run tests
		browser (karma, testem) - more config, slower
		headless browser (phantomjs) - no user interface
		in-memory dom (jsdom) - lighter weight alternative to simulate dom
	where to place tests
		centralized - mocha (avoids noise to source code); seperation does not makes senses in JS
		+alongside - 

		naming *.spec.js *.test.js
	when to run tests
		+unit tests should run every time the file is saved - rapid feedback, facilated tDD
		integration tests can be run separete

Continous integration
	+travis (linux) hosted solution
	+appveyor (windows)
	jenkins (alt popular option) self hosted
	circle ci
	sempahore
	snapci

HTTP Calls

  Node
    http | low level
    +request | higher level
  
  Browser
    XMLHttpRequest - native way to be done
    jquery - logical if jquery is used
    framework based - angular
    +Fetch - standar proposed, not everybody natively supports. use polyfill (isomorphic)

  Node & browser (file size or features)
    isomorphic-fetch
    xhr (npm package)
    super-agent (good framework)
    axios (clean promised based api)

    for specific browsers polyfill.io

  nock - for mocking http
  api-mock
  json-server (fake db using static json)
  json schema faker (generates fake data) good for catching edge cases with random data
  faker.js
  chance.js
  randexp.js
  

