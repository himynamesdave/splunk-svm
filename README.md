# splunk-svm
Splunk startup and shutdown script for demo / test environments

## Installing

First, set user variables in svm script. Example below:

```
TARDIR="/Users/dgreenwood/splunks/images" # where Splunk tgz image can be found
TARNAME="splunk-6.5.0-59c8927def0f-darwin-64.tgz" # tgz file name
INSTDIR="/Users/dgreenwood/splunks/environments" # dir where you want to run Splunk
NEWPORTFILE="/Users/dgreenwood/splunks"
BROWSER="chrome"
```

## Using

svm create INSTANCE_NAME - create new instance
svm start INSTANCE_NAME - starts the specified instance
svm stop INSTANCE_NAME - stops the specified instance
svm stopall - stops all running instances
svm restart INSTANCE_NAME - restarts the specified instance
svm open INSTANCE_NAME - opens the specified instance
svm clean - pkill the python and splunkd's running
svm delete INSTANCE_NAME - delete specified instance

## Examples

`sh sv create my_new_instance` Creates new instance called `my_new_instance`
`sh sv start my_new_instance` Starts instance called `my_new_instance`