# kanboard

![Version: 0.1.3](https://img.shields.io/badge/Version-0.1.3-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 1.2.18](https://img.shields.io/badge/AppVersion-1.2.18-informational?style=flat-square)

A free and open source Kanban project management software.

## Requirements

| Repository | Name | Version |
|------------|------|---------|
| https://nicholaswilde.github.io/helm-charts/ | common | ~0.1.8 |

## TL;DR
```console
$ helm repo add nicholaswilde https://nicholaswilde.github.io/helm-charts/
$ helm repo update
$ helm install kanboard nicholaswilde/kanboard
```

## Installing the Chart
To install the chart with the release name `kanboard`:
```console
helm install kanboard nicholaswilde/kanboard
```

## Uninstalling the Chart
To uninstall the `kanboard` deployment:
```console
helm uninstall kanboard
```
The command removes all the Kubernetes components associated with the chart and deletes the release.

## Configuration

Read through the [values.yaml](./values.yaml) file. It has several commented out suggested values.
Other values may be used from the [values.yaml](../common/values.yaml) from the [common library](../common).

Specify each parameter using the `--set key=value[,key=value]` argument to `helm install`. For example,
```console
helm install kanboard \
  --set env.TZ="America/New York" \
    nicholaswilde/kanboard
```

Alternatively, a YAML file that specifies the values for the above parameters can be provided while installing the chart.
For example,
```console
helm install kanboard nicholaswilde/kanboard -f values.yaml
```

## Author
This project was started in 2020 by [Nicholas Wilde](https://github.com/nicholaswilde).

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.5.0](https://github.com/norwoodj/helm-docs/releases/v1.5.0)