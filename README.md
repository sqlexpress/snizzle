# Snizzle
![npm version](https://img.shields.io/npm/v/snizzle)
![license](https://img.shields.io/github/license/jqrony/snizzle)
[![install size](https://packagephobia.com/badge?p=snizzle)](https://packagephobia.com/result?p=snizzle)
![author](https://img.shields.io/badge/Author-Shahzada%20Modassir-%2344cc11)

__A pure-JavaScript CSS selector engine designed to be easily dropped in to a host library.__

- [More information](https://snizzlejs.com/)
- [Documentation](https://github.com/jqrony/snizzle/wiki/)
- [Browser support](https://github.com/jqrony/snizzle/wiki/#wiki-browsers)

## License
- [MIT License](https://github.com/jqrony/snizzle/blob/1.3.0/LICENSE.txt)

What you need to build Snizzle
---------------------------

In order to build Snizzle, you should have Node.js/npm latest and git 1.7 or later (earlier versions might work OK, but are not tested).

For Windows you have to download and install [git](http://git-scm.com/downloads) and [Node.js](https://nodejs.org/download/).

Mac OS users should install [Homebrew](http://mxcl.github.com/homebrew/). Once Homebrew is installed, run `brew install git` to install git,
and `brew install node` to install Node.js.

Linux/BSD users should use their appropriate package managers to install git and Node.js, or build from source
if you swing that way. Easy-peasy.


How to build Snizzle
----------------------------

Clone a copy of the main Snizzle git repo by running:

```bash
git clone git://github.com/jqrony/snizzle.git
```

In the `snizzle/dist` folder you will find build version of snizzle along with the minified copy and associated map file.

Testing
----------------------------

- Run `npm install`, it's also preferable (but not necessarily) to globally install `grunt-cli` package – `npm install -g grunt-cli`
- Open `test/index.html` in the browser. Or run `npm test`/`grunt test` on the command line, if environment variables `BROWSER_STACK_USERNAME` and `BROWSER_STACK_ACCESS_KEY` are set up, it will attempt to use [Browserstack](https://www.browserstack.com/) service (you will need to install java on your machine so browserstack could connect to your local server), otherwise [PhantomJS](http://phantomjs.org/) will be used.
- The actual unit tests are in the `test/unit` directory.

Developing with [grunt](http://gruntjs.com)
----------------------------

- `npm run build` or `grunt` will lint, build, test, and compare the sizes of the built files.
- `npm start` or `grunt start` can be run to re-lint, re-build, and re-test files as you change them.
- `grunt -help` will show other available commands.
