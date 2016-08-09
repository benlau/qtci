#!/bin/bash

set -e

INFOPLIST_FILE=`xcodebuild -showBuildSettings | grep INFOPLIST_FILE | sed -e "s/.*=//g"`
buildNumber=`/usr/libexec/PlistBuddy -c "Print CFBundleVersion" $INFOPLIST_FILE`
buildNumber=$(($buildNumber+1))
xcrun agvtool new-version -all $buildNumber
