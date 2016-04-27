# QT-CI
A set of scripts to install Qt/Android by official installer in Linux command line environment (e.g travis/drone)

[![Build Status](https://travis-ci.org/benlau/qtci.svg?branch=master)](https://travis-ci.org/benlau/qtci)

Check [.travis.yml](https://github.com/benlau/qtci/blob/master/.travis.yml) to see how it works. 
It will demonstrate how to build a apk file using QT-CI scripts.

Commands
--------

**(1) bin/extract-qt-installer**

Extract installer of Qt to target path (for Qt 5.5 or above)

Example:

	extract-qt-installer qt-opensource-linux-x64-android-5.5.1.run ~/Qt

**(2) bin/extract-ifw**

Extract installer of "Qt installer framework" to target path

Example:

	extract-ifw qt-installer-framework-opensource-1.5.0-x64.run ~/QtIfw

**(3) bin/install-android-sdk**

Download and install Android SDK

Example:

	install-android-sdk platform-tool,build-tools-20.0.0,android-19

Related Projects
----------------

 1. [benlau/quickpromise](https://github.com/benlau/quickpromise) - Promise library for QML
 2. [benlau/quickcross](https://github.com/benlau/quickcross) - QML Cross Platform Utility Library
 3. [benlau/qsyncable](https://github.com/benlau/qsyncable) - Synchronize data between models
 4. [benlau/testable](https://github.com/benlau/testable) - QML Unit Test Utilities
 5. [benlau/quickflux](https://github.com/benlau/quickflux) - Message Dispatcher / Queue for Qt/QML
 6. [benlau/biginteger](https://github.com/benlau/biginteger) - QML BigInteger library
