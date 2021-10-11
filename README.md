# lumen-serverless-demo
Demo Severless Config Files for Use into a Laravel or Lumen project
[Tutorial for Lumen Serverless ](https://medinazdago.medium.com/soluci%C3%B3n-serverless-para-lumen-laravel-en-aws-con-bref-6bf276d26dc1)

# Serverless

## Installation
Main documentation links:

[Bref Laravel](https://bref.sh/docs/frameworks/laravel.html)

[Deploy Serverless Laravel](https://dev.to/chandreshhere/deploy-serverless-laravel-application-using-bref-cp2)

[Installation and AWS Configs](https://bref.sh/docs/installation.html)


If you don't has this libs, add it with the next commands, if not, only runs composer install normally

``` shell
npm install -g serverless

serverless config credentials --profile PROFILE_NAME --provider aws --key KEY --secret KEY

composer require bref/bref bref/laravel-bridge --update-with-dependencies
```

## Deploy Commands
#### Remember to change to master branch and git pull origin master
``` shell

serverless deploy --aws-profile PROFILE_NAME

#to remove
serverless remove --aws-profile PROFILE_NAME
