# glueops-prometheus-alerts

![Version: 0.1.0-alpha1](https://img.shields.io/badge/Version-0.1.0--alpha1-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 1.16.0](https://img.shields.io/badge/AppVersion-1.16.0-informational?style=flat-square)

A Helm chart for Kubernetes

## Requirements

| Repository | Name | Version |
|------------|------|---------|
| https://helm.gpkg.io/service | prometheus-alertmanagerconfig-opsgenie | v0.1.0 |

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| prometheus-alertmanagerconfig-opsgenie.labels | object | `{"alertname":"nil","component":"nil","team":"nil"}` | These labels are additional filters you can use to keep these notifications for one particular team, component, or alert. Note: you must set the same filters (with the exception of alertname) on the alert definition itself. The alert definition is also refered to as the prometheusrule. |
| prometheus-alertmanagerconfig-opsgenie.opsgenie.apikey | string | `"nil"` | Leave this value as `nil` if you provided a `vault_path`. Otherwise, this value must be set. You CANNOT have a `vault_path` and `opsgenie.apikey` defined at the same time. |
| prometheus-alertmanagerconfig-opsgenie.route | object | `{"groupInterval":"60m","repeatInterval":"60m"}` | Amount of time to fire an alert again after the first one is sent. |
