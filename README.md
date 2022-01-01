# Verify

Get user

```
kubectl --namespace jenkins get secret jenkins-operator-credentials-jenkins -o 'jsonpath={.data.user}' | base64 -d
```

Get Password

```
kubectl --namespace jenkins get secret jenkins-operator-credentials-jenkins -o 'jsonpath={.data.password}' | base64 -d
```

```
kubectl --namespace jenkins port-forward jenkins-jenkins 8080:8080
```