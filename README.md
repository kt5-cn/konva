Before doing all dev stuff make sure you have node installed. After that, run `npm install` in the main directory to install the node module dependencies.

Run `grunt --help` to see all build options.

#Building the KineticJS Framework 

To build a development version of the framework, run `grunt dev`. To run a full build, which also produces the minified version and the individually minified modules for the custom build, run `grunt full`.  You can also run `grunt beta` to generate a beta version.   

If you add a file in the src directory, be sure to add the filename to the sourceFiles array variable in Gruntfile.js.

#Testing

[![Build Status](https://travis-ci.org/ericdrowell/KineticJS.png)](https://travis-ci.org/ericdrowell/KineticJS)

KineticJS uses Mocha for testing. 

* If you need run test only one time run `grunt test`.
* While developing it is easy to use `grunt server` with watch task. Just run in in go to http://localhost:8080/test/runner.html. After src file change kinetic-dev.js will be automatically created, so you need just refresh test page.

KineticJS is covered with hundreds of tests and well over a thousand assertions.  KineticJS uses TDD (test driven development) which means that every new feature or bug fix is accompanied with at least one new test. 

#Generation documentation

`grunt gen-doc`


#Pull Requests
I'd be happy to review any pull requests that may better the KineticJS project, in particular if you have a bug fix, enhancement, or a new shape (see `src/shapes` for examples).  Before doing so, please first make sure that all of the tests pass (`grunt test`). 
