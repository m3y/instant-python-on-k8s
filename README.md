# instant-python-on-k8s
No need for image build

```
kind create cluster --name instant-python --config kluster.yaml
kustomize build . | kubectl apply -f -
kubectl logs -lapp=instant-python
```

See the following article
- https://blog.sakashita.dev/2020/11/pythonmd.html
