#!/bin/sh

export DISPLAY=:0
export DBUS_SESSION_BUS_ADDRESS="unix:path=/run/user/1000/bus"

grim -g "$(slurp -p)" -t ppm - | magick - -format '%[pixel:p{0,0}]' txt:- | tail -n 1 | cut -d ' ' -f 4 | wl-copy
if [ "$(wl-paste)" != "" ]; then
  notify-send "Copied $(wl-paste) to clipboard." -h string:frcolor:$(wl-paste)
fi
