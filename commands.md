# control minikube

```
$ minikube start
$ minikube dashboard

$ minikube stop
$ minikube delete
```

# create object

```
$ kubectl apply -f <file name>
```

# Deployment

```
// 過去の履歴の確認
$ kubectl rollout history deployment.v1.apps/nginx

// rollbackの実行
$ kubectl rollout undo deployment.v1.apps/nginx --to-revision=2

$ kubectl delete -f deployment.yaml
```

# ConfigMap

