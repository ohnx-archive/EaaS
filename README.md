# EaaS
[![Build Status](https://travis-ci.org/ohnx/EaaS.svg?branch=master)](https://travis-ci.org/ohnx/EaaS)
[![Dependencies](https://david-dm.org/ohnx/EaaS.svg)](https://david-dm.org/ohnx/EaaS)

Error as a Service

## about
have you ever needed to display an error in your application, but had no idea what to say in it?

Look no further! EaaS is here!

EaaS (Error as a Service) provides a modern, RESTful, scalable solution to the common problem of needing an error message to display to a user[\[1\]](http://foaas.com/).

Returned error messages are taken from some of the tech industry's best error-producing companies and software (ie, Microsoft)!

Some other error messages are just error messages. After all, Windows and Unix only have a limited number of actually good error messages.

## usage
either run it on your own server with `node server.js`, or be a cheapo and use the one I'm hosting on [Red Hat OpenShift](https://www.openshift.com/) at the url [http://eaas.masonx.ca/](http://eaas.masonx.ca/)

## API
### getting an error
make a GET request to `/txt` or `/` to get an error message back in plaintext.

alternatively, you can also send a GET request to `/json` to get a JSON response.

## roadmap
 - [ ] allow selection of type of error message (ie, web, nix, win, misc, all) - quite hard
 - [ ] use [mongoDB](https://www.youtube.com/watch?v=dQw4w9WgXcQ) somehow to make this /really/ web-scale
 - [ ] Java Exception class that uses this

## contributing
Please donate your error messages! Fork the repo, add to the end of `errors.json` and make a pull request.
