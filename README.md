Heroku Buildpack for node/bower/gulp
========================================

Usage
-----
- Set your Heroku app's buildpack URL: 
```
heroku config:set BUILDPACK_URL=https://github.com/artmees/heroku-buildpack-nodejs-gulp-bower.git`
```
- Run `heroku config:set NODE_ENV={{env}}` to set your environment to the desired environment. 
  ex `production` or `staging`

-  Add a Gulp task called for each enviroment you support `heroku:{{env}}` that builds your app.
  ex `heroku:production` or `heroku:staging`

Credits
-------
* Forked from [heroku-buildpack-nodejs](https://github.com/heroku/heroku-buildpack-nodejs).
* Forked from [krry](https://github.com/krry/heroku-buildpack-nodejs-gulp-bower) awesome build back.
* Incorporated bower check and install from [heroku-buildpack-nodejs-gulp-bower](https://github.com/davidmfoley/heroku-buildpack-nodejs-gulp-bower)
* Heavily based on [heroku-buildpack-nodejs-grunt](https://github.com/mbuchetics/heroku-buildpack-nodejs-grunt).
