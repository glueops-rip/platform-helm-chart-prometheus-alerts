# glueops-prometheus-alerts

![Version: 0.4.0-antonio-alpha3](https://img.shields.io/badge/Version-0.4.0--antonio--alpha3-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 1.16.0](https://img.shields.io/badge/AppVersion-1.16.0-informational?style=flat-square)

A Helm chart for Kubernetes

## Requirements

| Repository | Name | Version |
|------------|------|---------|
| https://helm.gpkg.io/service | prometheus-alertmanagerconfig-opsgenie | v0.1.0 |

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| labels | object | `{"alertname":"nil","component":"nil","team":"nil"}` | These labels are additional filters you can use to keep these notifications for one particular team, component, or alert. Note: you must set the same filters (with the exception of alertname) on the alert definition itself. The alert definition is also refered to as the prometheusrule. |
