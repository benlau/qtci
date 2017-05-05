#!/bin/sh

if [ "$#" -ne 2 ]
then
    echo set-file-suffix file suffix
    exit -1
fi

NAME=`echo "$1" | cut -d'.' -f1`
EXTENSION=`echo "$1" | cut -d'.' -f2`

mv $1 ${NAME}-$2.$EXTENSION
