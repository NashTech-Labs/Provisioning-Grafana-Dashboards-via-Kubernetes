### Provisioning Dashboards in Grafana using Kubernetes yaml files

Fist of all using GrafanaInstanceConfig.yml we have created Grafana instance after that we have added a configMap. This will hold the configuration file for us in a centralized place. We have added three volumes 

- grafana-datasources
- grafana-dashboard
- grafana-dashboard-defintion

Using dashboardconfig.yml grafana will look every 10 seconds into the path /var/lib/grafana/dashboards and check if there is a new dashboard definition.
Finally using Dashboard.yml we have created a dashboard for grafana.
