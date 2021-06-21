Satorix Google Cloud SDK buildpack
===========================

Use [Google Cloud SDK](https://cloud.google.com/sdk) in a buildpack compatible app.

Requires
--------

Python 3 

Usage
-----

Add the buildpack to a `.buildpacks` configuration in the root of the application directory to install `gcloud` and `kubectl` for the application to utilize.

Configuration
-------------

* `GOOGLE_CLOUD_SDK_BIN_URL` set the source URL for the Google Cloud SDK
  * Defaults to 64-bit Linux binary for Heroku runtime
  * Expects a `*.tar.gz` file as [distributed by Google](https://cloud.google.com/sdk/docs/downloads-versioned-archives)
