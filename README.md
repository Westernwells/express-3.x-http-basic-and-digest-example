This example demonstrates how to use [Express](http://expressjs.com/) 3.x and
[Passport](http://passportjs.org/) to authenticate users via either the HTTP
Basic or HTTP Digest schemes.  Use this example as a starting point for your own
web applications.

## Instructions

To install this example on your computer, clone the repository and install
dependencies.

```bash
$ git clone git@github.com:passport/express-3.x-http-basic-and-digest-example.git
$ cd express-3.x-http-basic-and-digest-example
$ npm install
```

Start the server.

```bash
$ node server.js
```

Use `curl` to send an authenticated request using HTTP Basic scheme.

```bash
$ curl -v --user jack:secret --basic http://127.0.0.1:3000/
```

Use `curl` to send an authenticated request using HTTP Digest scheme.

```bash
$ curl -v --user jack:secret --digest http://127.0.0.1:3000/
```
