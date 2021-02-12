# instant-python-on-k8s
No need for image build

```
kind create cluster --name instant-python
kustomize build . | kubectl apply -f -
kubectl logs -lapp=instant-python
```
