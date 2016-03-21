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
