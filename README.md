# 19-VS
_This repo is for debugging purposes_

## Install Helm Chart
From the root directory of the repo.
```
helm install task .
```


## Uninstall Helm Chart
```
helm uninstall task
```


## Test Routes
Test 7
```
curl -H "HOST: jja" $(glooctl proxy url)/api/v1/test/7
```

Test 20
```
curl -H "HOST: wwa" $(glooctl proxy url)/api/v1/test/20
```

Check Health
```
curl $(glooctl proxy url)/api/v1/healthz
```