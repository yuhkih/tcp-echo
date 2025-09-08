# tcp-echo


Return the same string you enterl.

```
$ oc get svc
NAME       TYPE           CLUSTER-IP       EXTERNAL-IP                                                                    PORT(S)          AGE
tcp-echo   LoadBalancer   172.30.150.193   a4bb1d028fd02428e87b8d7ae9974f45-1101313903.ap-northeast-1.elb.amazonaws.com   9000:31079/TCP   95m
$ nc  a4bb1d028fd02428e87b8d7ae9974f45-1101313903.ap-northeast-1.elb.amazonaws.com 9000
aaa
aaa
hello!
hello!
^C
$ 
```
