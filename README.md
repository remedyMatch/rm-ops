# Operations Infrastruktur für Remedy Match

Alle Stacks wurden mit Portainer UI aufgesetzt.

## Monitoring & Alerting: Grafana und Prometheus
* Grafana: https://monitoring.remedymatch.io/grafana
  * User: admin
  * Password: Pa55w0rd
* Prometheus Server: https://monitoring.remedymatch.io/prometheus
* Prometheus Alert Manager: tbd

Im Moment offen: 
* Applikation Metriken senden lassen 

## Logging: ELK-Stack
* Bevor der Stack gestartet werden kann, müssen die vier Configs über die Portainer UI angelegt werden.
  * elasticserch-yml -> elastic_config
  * kibana.yml -> kibana_config
  * logstash.conf -> logstash_pipeline
  * logstash.yml -> logstash_config
* Kibana: https://monitoring.remedymatch.io/kibana/app/kibana#/home
  * User: elastic
  * Password: changemene
  * basiert auf https://github.com/deviantony/docker-elk

Im Moment offen: 
* Applikation Logs senden lassen 