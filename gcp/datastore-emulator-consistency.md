# Set Datastore Emulator Consistency 

The default consistency is set to 0.9, which is suboptimal value when running tests.
  
Value Can be adjusted via `--consistency` parameter, eg.:

```shell
$ gcloud beta emulators datastore start --consistency=1
```
