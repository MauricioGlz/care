# care 

Adds your awesome app description here!

(maybe adds a screenshot, people loves screenshots!)

## Get it from the elementary OS AppCenter!

[![Get it on AppCenter](https://appcenter.elementary.io/badge.svg)](https://appcenter.elementary.io/care)

This app is available on the elementary OS AppCenter.

# Install it from source

You can of course download and install this app from source.

## Dependencies

Ensure you have these dependencies installed

* granite
* gtk+-3.0
* switchboard-2.0

## Install, build and run

```bash
# install elementary-sdk, meson and ninja 
sudo apt install elementary-sdk meson ninja
# clone repository
git clone {{repository_url}} care
# cd to dir
cd care
# run meson
meson build --prefix=/usr
# cd to build, build and test
cd build
sudo ninja install && care
```

## Generating pot file

```bash
# after setting up meson build
cd build

# generates pot file
sudo ninja care-pot

# to regenerate and propagate changes to every po file
sudo ninja care-update-po
```
