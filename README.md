# A S3 Image Uploader

A barebones Node.js app using [Express 4](http://expressjs.com/).



## Prerequisites

Make sure you have [Node.js](http://nodejs.org/) and the [Heroku CLI](https://cli.heroku.com/) installed.
An AWS S3 bucket has been created;
You have AWS authentication keys that have write access to the bucket.

## Running Locally


```sh
$ git clone git@github.com:vikasbguru/awschatbot-unleashed.git # or clone your own fork
$ cd uploadimages
$ npm install
$ npm start
```

Your app should now be running on [localhost:5000](http://localhost:5000/).

## Deploying to Heroku

```
$ heroku create
$ git push heroku master
$ heroku ps:scale web=1
$ heroku config:set AWS_ACCESS_KEY_ID=xxx AWS_SECRET_ACCESS_KEY=yyy
$ heroku config:set S3_BUCKET=zzz
$ heroku open
```
or

[![Deploy to Heroku](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy)
