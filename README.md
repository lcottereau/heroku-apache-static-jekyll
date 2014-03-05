Apache serving a generated static jekyll site
========================

This is a build pack bundling Apache for serving static pages generated with Jekyll on Heroku. Redirections will be allowed (we'll see if we have to activate `.htaccess`).

Configuration
-------------

The config files are bundled with the build pack itself:

* conf/httpd.conf


Pre-compiling binaries
----------------------

See [the official PHP Heroku Buildpack](https://github.com/heroku/heroku-buildpack-php#pre-compiling-binaries)

Hacking
-------

To change this buildpack, fork it on Github. Push up changes to your fork, then create a test app with --buildpack <your-github-url> and push to it.


Meta
----

Forked from [the official PHP Heroku Buildpack](https://github.com/heroku/heroku-buildpack-php)
