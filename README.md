# Heroku Buildpack for Ghostscript

Currently installs Ghostscript 10.08.0 on Heroku Cedar.

## Install

    # Use heroku-buildpack-multi
    $ cd /path/to/your-app
    $ heroku config:add BUILDPACK_URL=https://github.com/ddollar/heroku-buildpack-multi.git

    # Create a .buildpacks file with including ghostscript
    $ cd /path/to/your-app
    $ cat .buildpacks
    https://github.com/heroku/heroku-buildpack-ruby.git
    https://github.com/elbongurk/heroku-buildpack-ghostscript.git

    # Push changes to deploy
    $ git push
