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

課題：replicaset や deployment から configMap を読み込む

# secret

```
// encode
$ echo -n 'admin' | base64
// 結果 → YWRtaW4=

// decode
$ echo -n 'YWRtaW4=' | base64 --decode
// 結果 → admin
```
