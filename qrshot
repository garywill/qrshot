#!/bin/bash

if [[ ! "$1" ]]; then

    TMPDIR=/dev/shm
    cd "$TMPDIR"

    echo Use mouse select an area on screen to decode QR
    echo ""

    scrot -s -e 'echo Image size $w x $h ; echo "" ; zbarimg "$f" ; rm  "$f" '

else
    qrencode -m 2 -t ANSIUTF8 "$1"
fi
