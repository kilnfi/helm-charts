# teku-beacon

![Version: 0.3.1](https://img.shields.io/badge/Version-0.3.1-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 22.5.0-jdk17](https://img.shields.io/badge/AppVersion-22.5.0--jdk17-informational?style=flat-square)

A Helm chart for Teku Ethereum Beacon Chain

## Maintainers

| Name | Email | Url |
| ---- | ------ | --- |
| kiln | <contact@kiln.fi> |  |

## Source Code

* <https://github.com/ConsenSys/teku>

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| affinity | object | `{}` |  |
| autoscaling.enabled | bool | `false` |  |
| autoscaling.maxReplicas | int | `100` |  |
| autoscaling.minReplicas | int | `1` |  |
| autoscaling.targetCPUUtilizationPercentage | int | `80` |  |
| config | object | `{}` |  |
| env | object | `{}` |  |
| extraArgs | object | `{}` |  |
| fullnameOverride | string | `""` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.repository | string | `"consensys/teku"` |  |
| image.tag | string | `""` |  |
| imagePullSecrets | list | `[]` |  |
| jwtSecret | string | `""` |  |
| nameOverride | string | `""` |  |
| nodeSelector | object | `{}` |  |
| persistence.accessMode | string | `"ReadWriteOnce"` |  |
| persistence.enabled | bool | `true` |  |
| persistence.size | string | `"80Gi"` |  |
| podAnnotations | object | `{}` |  |
| podManagementPolicy | string | `"Parallel"` |  |
| podSecurityContext.fsGroup | int | `1000` |  |
| replicaCount | int | `1` |  |
| resources | object | `{}` |  |
| securityContext | object | `{}` |  |
| service.rpc.sessionAffinity | string | `"None"` |  |
| service.rpc.sessionAffinityConfig | object | `{}` |  |
| serviceAccount.annotations | object | `{}` |  |
| serviceAccount.create | bool | `true` |  |
| serviceAccount.name | string | `""` |  |
| serviceMonitor.additionalLabels | object | `{}` |  |
| serviceMonitor.enabled | bool | `false` |  |
| serviceMonitor.metricRelabelings | list | `[]` |  |
| serviceMonitor.namespace | string | `""` |  |
| serviceMonitor.namespaceSelector | object | `{}` |  |
| serviceMonitor.scrapeInterval | string | `"60s"` |  |
| serviceMonitor.targetLabels | list | `[]` |  |
| tolerations | list | `[]` |  |
| updateStrategyType | string | `"RollingUpdate"` |  |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.14.2](https://github.com/norwoodj/helm-docs/releases/v1.14.2)
