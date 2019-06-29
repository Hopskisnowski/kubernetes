# How to build
```
 oc delete dc myp
 docker images
 GOOS=linux go build -o ./app .
 docker build -t in-cluster .
 docker images
 docker rmi 115250a5e1c9
 oc run -i myp --image=in-cluster --image-pull-policy=Never
 oc get pods
 oc log myp-1-mgxtj
 oc delete dc myp 
```
