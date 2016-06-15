# Hidden settings

Turn on context menu (i.e. right click) for native apps built with web views
```
defaults write NSGlobalDomain WebKitDeveloperExtras -bool true
```

Turn off drop shadows when taking screenshots
```
defaults write com.apple.screencapture disable-shadow -bool true
killall SystemUIServer
```

View all files downloaded, as logged via your favorite web browser (see [link](http://lifehacker.com/your-mac-logs-everything-you-download-heres-how-to-cle-1658394180))
```
sqlite3 ~/Library/Preferences/com.apple.LaunchServices.QuarantineEventsV* 'select LSQuarantineDataURLString from LSQuarantineEvent'
```

Delete above log:
```
sqlite3 ~/Library/Preferences/com.apple.LaunchServices.QuarantineEventsV* 'delete from LSQuarantineEvent'
```
