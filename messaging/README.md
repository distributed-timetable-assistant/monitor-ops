```bash
helm repo add redpanda https://charts.redpanda.com
```

```bash
helm repo update
```

```bash
helm upgrade --install redpanda-controller redpanda/operator \                                                                                                                                                      130 ↵
  --namespace redpanda-system \
  --create-namespace \
  --set crds.enabled=true
```