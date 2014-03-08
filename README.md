Static Jekyll Buildpack
========================

This is a build pack bundling Apache for serving static pages generated with Jekyll on Heroku. It allows you to simply commit your jekyll sources and let heroku do all the compiling.

As of now (but I will change it), I still simply allow `.htaccess` files in the sources, so that redirections can be implemented and saved with the rest of the site sources, but (for performance sake) I will change the way this is done at some point (but redirections will still be allowed).

You can look at [my personal site](https://github.com/lcottereau/name.cottereau.laurent) to see how this can be used.

Configuration
-------------

The config files are bundled with the build pack itself:

* conf/httpd.conf


Pre-compiling binaries
----------------------

See [the official PHP Heroku Buildpack](https://github.com/heroku/heroku-buildpack-php#pre-compiling-binaries)

Hacking
-------

To use this buildpack directly, you can just execute

    heroku config:set BUILDPACK_URL=https://github.com/lcottereau/heroku-apache-static-jekyll

To change this buildpack, fork it on Github. Push up changes to your fork, then create a test app with --buildpack <your-github-url> and push to it. You can also 


Meta
----

Forked from [the official PHP Heroku Buildpack](https://github.com/heroku/heroku-buildpack-php)
