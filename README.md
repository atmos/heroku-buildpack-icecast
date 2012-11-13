Icecast on Heroku
=================

Because why the fuck would you wanna pay for bandwidth to stream to folks?

This is a heroku buildpack that runs an icecast server that's friendly to the
heroku environment.  If you use it, it requires a `config/icecast.xml` file to
be in your heroku application's directory structure.

This is still pretty hacky and experimental, and requires some SSL load
balancer options that heroku doesn't offer by default right now.

Installation
------------

  * Create your heroku application
  * Supply the `BUILDPACK_URL` env variable 

```
heroku config:add BUILDPACK_URL="BUILDPACK_URL: https://github.com/atmos/heroku-buildpack-icecast.git"
```

Modify your configuration file to suit your needs.  Enjoi.
