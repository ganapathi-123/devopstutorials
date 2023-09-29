# Most Common Kubernetes Deployment Strategies


## Test application

```bash
kubectl kubectl run -it --rm --image=curlimages/curl curly -- sh
for i in `seq 1 1000`; do curl myapp.default:8181/version; echo ""; sleep 1; done
```