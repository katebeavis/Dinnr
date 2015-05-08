[![Build Status](https://travis-ci.org/Dinnr-Makers/Dinnr.svg?branch=master)](https://travis-ci.org/Dinnr-Makers/Dinnr)
[![Code Climate](https://codeclimate.com/github/Dinnr-Makers/Dinnr/badges/gpa.svg)](https://codeclimate.com/github/Dinnr-Makers/Dinnr)
[![Test Coverage](https://codeclimate.com/github/Dinnr-Makers/Dinnr/badges/coverage.svg)](https://codeclimate.com/github/Dinnr-Makers/Dinnr)
# Dinnr
Dinnr was built as a two week final project at Makers Academy. It is a social app for organising dinner parties with friends and strangers, similar to Airbnb.

Users can sign up and log in through email or Facebook and receive confirmation emails. They are able to create events, join and leave events, leave comments and reviews.

## Heroku & Screenshots
###[Dinnr](http://dinnr.herokuapp.com)
<div align="center">
  <img width="90%" src="app/assets/images/dinnr-top.png">
</div>
<div align="center">
  <img width="90%" src="public/img/orange-thermo.png">
</div>
<div align="center">
  <img width="90%" src="public/img/orange-thermo.png">
</div>
<div align="center">
  <img width="90%" src="public/img/orange-thermo.png">
</div>

## Objectives
We wanted to create an app to bring people together - one of the members of our team had moved to London a few months beforehand, and he wanted a site where he could organise a dinner party at his house in order to meet new people.

## Todo
##### Payment System
We wanted to implement a payment system where guests could leave a deposit for the party they were going to attend. This was to be done through Stripe but unfortunately it didn't fit the time constraints of our project.
##### Search/Tags by dietary requirement
The next thing on our list was to create a search which would filter events by dietary requirement. We also thought it would be a nice touch to have tags, similar to those on blogs that could be attached to an event.
##### Badges (Gamification)
This was far off in the backlog but I loved the idea of 'gamifying' the experience through the awarding of badges. For example if your event had a certain number of positive reviews or you had attended a certain number of events, you would be awarded a badge.

## To Run

```
$ git clone https://github.com/katebeavis/Dinnr.git
$ cd Dinnr
```

- [Image Magick](http://www.imagemagick.org/script/binary-releases.php) needs to be installed in advance
- Postgresql
- You need to set up the following environment variables in a `.env` file in the root directory:
  <br>```GMAIL_DOMAIN=gmail.com
  GMAIL_USERNAME=dinnr.maker@gmail.com
  GMAIL_PASSWORD=XXXXX_YOUR_PASSWORD_XXX
  FACEBOOK_APP_SECRET=XXX_YOUR_FB_SECRET_XXXX
  AWSSecretKey=XXX_YOUR_AMAZON_WEB_SERVICES_KEY_XXX
  AWSAccessKeyId=XXX_YOUR_AWS_ID_XXXX```

```
$ bundle install
$ bower install
$ rake db:create db:migrate
$ rails s
```

## Run tests
```
$ rspec
```

#On Windows:
We included a third environment for Windows development. To run the server in this environment run ```rails s -e development_windows```. In the other environments photo upload won't work on Windows machines. This is because the Rmagick gem doesn't work on Windows machines. In development_windows environment photos get processed by ImageMagick instead. If it doesn't work properly, please check if the path to ImageMagick in ```config/environments/development_windows``` are correct for your ImageMagick installation:

```Paperclip.options[:command_path] = "C:\\Program\ Files\\ImageMagick-6.9.1-Q16"
Paperclip.options[:command_path] = "C:\\Program\ Files (x86)\\GnuWin32\\bin"```
