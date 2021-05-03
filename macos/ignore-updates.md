# Ignore Updates Selectively

```shell
$ sudo softwareupdate --ignore "macOS Catalina"
$ defaults write com.apple.systempreferences AttentionPrefBundleIDs 0
$ killall Dock
```


### reset back to default 
```shell
$ sudo softwareupdate --reset-ignored
```