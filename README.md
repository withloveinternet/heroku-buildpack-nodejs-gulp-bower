Heroku Buildpack for node/bower/gulp
========================================

Usage
-----
1. Set your Heroku app's buildpack URL: `heroku config:set BUILDPACK_URL=https://github.com/krry/heroku-buildpack-nodejs-gulp-bower.git`
2. Run `heroku config:set NODE_ENV=production` to set your environment to `production`
3. Add a Gulp task called `heroku:production` that builds your app for production purposes

Credits
-------
* Forked from [heroku-buildpack-nodejs](https://github.com/heroku/heroku-buildpack-nodejs).
* Incorporated bower check and install from [heroku-buildpack-nodejs-gulp-bower](https://github.com/davidmfoley/heroku-buildpack-nodejs-gulp-bower)
* Heavily based on [heroku-buildpack-nodejs-grunt](https://github.com/mbuchetics/heroku-buildpack-nodejs-grunt).
