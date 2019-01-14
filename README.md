# Building wheels for biolab/orange3 wheels

[![Appveyor](https://ci.appveyor.com/api/projects/status/vt0uk3tbrw2fr8lm?svg=true)](https://ci.appveyor.com/project/ales-erjavec/orange3-wheels)
[![Travis](https://travis-ci.org/ales-erjavec/orange3-wheels.svg?branch=master)](https://travis-ci.org/ales-erjavec/orange3-wheels)

The Windows and macOS wheels are build on appveyor and travis CI systems

To make/build a new release, edit the appveyor.yml and .travis.yml files and
change the `BUILD_COMMIT` version to the appropriate tag/ref in the orange3
git repository. Commit the changes and push the this repo (or create a pull
request and have someone merge it). Once the changes are pushed the builds on
appveyor and travis will be automatically started.

After the wheels are build they are uploaded to
[anaconda.org](https://anaconda.org/ales-erjavec/orange3/files)

The windows wheels are also stored as build artifacts on appveyor. For macOS
the wheels are also uploaded/shared (for a limited time) using transfer.sh
service. Look for the url in the travis log near the end.
