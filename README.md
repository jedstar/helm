##create fleet.yaml

```
defaultNamespace: default
helm:
  repo: https://jedstar.github.io/helm/
  chart: app-template
  values:
    clusterName: global.fleet.clusterLabels.management.cattle.io/cluster-display-name
  valuesFiles:
      - values.yaml
```

copy `charts/default-app/values.yaml` and modify as needed 