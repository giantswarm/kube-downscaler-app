# kube-downscaler

Downscaling tool to save on resources with dev clusters when they are not used

**Homepage:** <https://github.com/giantswarm/kube-downscaler-app>

## Source Code

* <https://github.com/caas-team/py-kube-downscaler>

## Requirements

| Repository | Name | Version |
|------------|------|---------|
| https://caas-team.github.io/helm-charts/ | kube-downscaler(py-kube-downscaler) | 0.3.12 |

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| enabled | bool | `false` |  |
| ciliumNetworkPolicy.enabled | bool | `true` |  |
| daemonset.downscale | bool | `false` |  |
| daemonset.job.image.registry | string | `"docker.io"` |  |
| daemonset.job.image.name | string | `"giantswarm/kubectl"` |  |
| daemonset.job.image.tag | string | `"1.28.4"` |  |
| daemonset.job.image.pullPolicy | string | `"IfNotPresent"` |  |
| daemonset.job.downscaleSchedule | string | `"0 2 * * 6"` |  |
| daemonset.job.upscaleSchedule | string | `"0 22 * * 7"` |  |
| daemonset.list | list | `[]` |  |
| kube-downscaler.image.repository | string | `"gsoci.azurecr.io/giantswarm/py-kube-downscaler"` |  |
| kube-downscaler.image.pullPolicy | string | `"IfNotPresent"` |  |
| kube-downscaler.image.tag | string | `"26.4.0"` |  |
| kube-downscaler.arguments[0] | string | `"--interval=60"` |  |
| kube-downscaler.arguments[1] | string | `"--include-resources=deployments,statefulsets,scaledobjects,horizontalpodautoscalers"` |  |
| kube-downscaler.serviceAccount.create | bool | `true` |  |
| kube-downscaler.serviceAccount.name | string | `""` |  |
| kube-downscaler.excludedNamespaces | list | `[]` |  |
| kube-downscaler.configMapName | string | `"kube-downscaler"` |  |
| kube-downscaler.extraConfig | string | `"DOWNSCALE_PERIOD: \"Sat-Sat 02:00-24:00 CET,Sun-Sun 00:00-22:00 CET\"\nDOWNTIME_REPLICAS: 1\n"` |  |
| kube-downscaler.securityContext.runAsNonRoot | bool | `true` |  |
| kube-downscaler.securityContext.runAsUser | int | `1000` |  |
| kube-downscaler.securityContext.runAsGroup | int | `1000` |  |
| kube-downscaler.securityContext.readOnlyRootFilesystem | bool | `true` |  |
| kube-downscaler.securityContext.allowPrivilegeEscalation | bool | `false` |  |
| kube-downscaler.securityContext.capabilities.drop[0] | string | `"ALL"` |  |
| kube-downscaler.securityContext.seccompProfile.type | string | `"RuntimeDefault"` |  |
| kube-downscaler.podSecurityContext.fsGroup | int | `1000` |  |
| kube-downscaler.podSecurityContext.runAsGroup | int | `1000` |  |
| kube-downscaler.podSecurityContext.runAsNonRoot | bool | `true` |  |
| kube-downscaler.podSecurityContext.runAsUser | int | `1000` |  |
| kube-downscaler.podSecurityContext.seccompProfile.type | string | `"RuntimeDefault"` |  |
