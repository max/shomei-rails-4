# Shomei

A simple NDA and signature pad app for [Heroku](https://www.heroku.com/):

![http://cl.ly/image/3W3X1U2l390p](http://cl.ly/image/3W3X1U2l390p/content#.png)

## Installing locally

To run this app locally you need Ruby 1.9.3 and Postgres.

```
$ bundle install
$ cp config/database.example.yml config/database.yml
$ bundle exec rake db:create
$ bundle exec rake db:migrate
$ foreman start
```

## Deploying to Heroku

```
$ heroku create
$ git push heroku master
$ heroku run rake db:migrate
```
