# gotify

a simple server for sending and receiving messages

![Version: 0.1.0](https://img.shields.io/badge/Version-0.1.0-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 2.0.20](https://img.shields.io/badge/AppVersion-2.0.20-informational?style=flat-square)

## TL;DR
```console
$ helm repo add nicholaswilde https://nicholaswilde.github.io/helm-charts/
$ helm repo update
$ helm install gotify nicholaswilde/gotify
```

## Installing the Chart
To install the chart with the release name `gotify`:
```console
helm install gotify nicholaswilde/gotify
```

## Uninstalling the Chart
To uninstall the `gotify` deployment:
```console
helm uninstall gotify
```
The command removes all the Kubernetes components associated with the chart and deletes the release.

## Configuration

Read through the [values.yaml](https://github.com/nicholaswilde/helm-charts/blob/master/charts/gotify/values.yaml)
file. It has several commented out suggested values.

Specify each parameter using the `--set key=value[,key=value]` argument to `helm install`. For example,
```console
helm install gotify \
  --set env.TZ="America/New York" \
    nicholaswilde/gotify
```

Alternatively, a YAML file that specifies the values for the above parameters can be provided while installing the chart.
For example,
```console
helm install gotify nicholaswilde/gotify --values values.yaml
```

## Author
This project was started in 2020 by Nicholas Wilde.

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.4.0](https://github.com/norwoodj/helm-docs/releases/v1.4.0)
