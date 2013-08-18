#!/usr/bin/env bash

echo "\nInstally dexron for Transmissions in $HOME/Library/Application\ Support/Transmission/scripts"
SCRIPTDIR = "$HOME/Library/Application\ Support/Transmission/scripts"
mkdir -p "$SCRIPTDIR"
curl -o "$HOME/Library/Application\ Support/Transmission/scripts/dexron" https://raw.github.com/mmoss/dexron/master/dexron

echo "\nSetting dexron to run automatically when a file completes downloading"
defaults write org.m0k.transmission DoneScriptEnabled -bool TRUE
defaults write org.m0k.transmission DoneScriptPath "$SCRIPTDIR/dexron"

echo "\nInstallation complete. Restart Transmission for dexron to run automatically."
