# QT-CI
A set of scripts to install Qt in Linux command line environment

[![Build Status](https://travis-ci.org/benlau/qtci.svg?branch=master)](https://travis-ci.org/benlau/qtci)

Check .travis.yml to see how it works

Commands
--------

**(1) bin/extract-qt-installer**

Extract installer of Qt to target path

Example:

	extract-qt-installer qt-opensource-linux-x64-android-5.5.1.run ~/Qt

**(2) bin/extract-ifw**

Extract installer of "Qt installer framework" to target path

Example:

	extract-ifw qt-installer-framework-opensource-1.5.0-x64.run ~/QtIfw
