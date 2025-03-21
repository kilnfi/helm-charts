# erigon

![Version: 7.0.1](https://img.shields.io/badge/Version-7.0.1-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: v2.39.0](https://img.shields.io/badge/AppVersion-v2.39.0-informational?style=flat-square)

A Helm chart for Erigon Ethereum Execution Layer client

## Maintainers

| Name | Email | Url |
| ---- | ------ | --- |
| kiln | <contact@kiln.fi> |  |

## Source Code

* <https://github.com/ledgerwatch/erigon>

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| affinity | object | `{}` |  |
| autoscaling.enabled | bool | `false` |  |
| autoscaling.maxReplicas | int | `100` |  |
| autoscaling.minReplicas | int | `1` |  |
| autoscaling.targetCPUUtilizationPercentage | int | `80` |  |
| autoscaling.targetMemoryUtilizationPercentage | int | `80` |  |
| customGenesis | string | `""` |  |
| erigon.datadir | string | `"/home/erigon/.local/share/erigon"` |  |
| erigon.enabled | bool | `true` |  |
| erigon.extraArgs | object | `{}` |  |
| erigon.resources | object | `{}` |  |
| erigon.securityContext | string | `nil` |  |
| fullnameOverride | string | `""` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.repository | string | `"thorax/erigon"` |  |
| image.tag | string | `""` |  |
| imagePullSecrets | list | `[]` |  |
| ingress.annotations | object | `{}` |  |
| ingress.className | string | `""` |  |
| ingress.enabled | bool | `false` |  |
| ingress.hosts[0].host | string | `"chart-example.local"` |  |
| ingress.hosts[0].paths[0].path | string | `"/"` |  |
| ingress.hosts[0].paths[0].pathType | string | `"ImplementationSpecific"` |  |
| ingress.tls | list | `[]` |  |
| jwtSecret | string | `""` |  |
| nameOverride | string | `""` |  |
| nodeSelector | object | `{}` |  |
| persistence.accessMode | string | `"ReadWriteOnce"` |  |
| persistence.enabled | bool | `true` |  |
| persistence.size | string | `"500Gi"` |  |
| podAnnotations | object | `{}` |  |
| podSecurityContext.fsGroup | int | `0` |  |
| podSecurityContext.runAsGroup | int | `0` |  |
| podSecurityContext.runAsUser | int | `0` |  |
| replicaCount | int | `1` |  |
| service.engine.port | int | `8551` |  |
| service.p2p.enableHostPort | bool | `true` |  |
| service.p2p.port | int | `30303` |  |
| service.rpc.port | int | `8545` |  |
| serviceAccount.annotations | object | `{}` |  |
| serviceAccount.create | bool | `true` |  |
| serviceAccount.name | string | `""` |  |
| serviceMonitor.additionalLabels | object | `{}` |  |
| serviceMonitor.enabled | bool | `false` |  |
| serviceMonitor.metricRelabelings | list | `[]` |  |
| serviceMonitor.namespace | string | `""` |  |
| serviceMonitor.namespaceSelector | object | `{}` |  |
| serviceMonitor.path | string | `"/debug/metrics/prometheus"` |  |
| serviceMonitor.scrapeInterval | string | `"60s"` |  |
| serviceMonitor.targetLabels | list | `[]` |  |
| tolerations | list | `[]` |  |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.14.2](https://github.com/norwoodj/helm-docs/releases/v1.14.2)
