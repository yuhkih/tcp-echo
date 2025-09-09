# tcp-echo


Return the same string you enter.


## 1. Get the elb name and the external listening port for your service
```
$ oc get svc
NAME       TYPE           CLUSTER-IP       EXTERNAL-IP                                                                    PORT(S)          AGE
tcp-echo   LoadBalancer   172.30.150.193   a4bb1d028fd02428e87b8d7ae9974f45-1101313903.ap-northeast-1.elb.amazonaws.com   9000:31079/TCP   95m
```

## 2. Access it using the nc command
```
$ nc  a4bb1d028fd02428e87b8d7ae9974f45-1101313903.ap-northeast-1.elb.amazonaws.com 9000
aaa
aaa
hello!
hello!
^C
$ 
```

With ROSA 4.18, CLB will be deployed for Sevice type=LoadBalancer
