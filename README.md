# How to 
## How to delete BC, running POD and image
```
 oc delete dc myp
```
## How to build Go app in local dir
```
 GOOS=linux go build -o ./app .
```
## How to build Docker container in local dir
```
 docker build -t in-cluster .
```
## How to run image in local MiniShift
```
 oc run -i myp --image=in-cluster --image-pull-policy=Never
```
## How to watch log
```
 oc get pods
 oc log myp-1-mgxtj
```
