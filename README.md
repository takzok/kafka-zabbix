# Kafka-prometheus

Docker-compose file for Apache Kafka metrics monitoring verification using zabbix.

## Containers

This docker-compose contains following containers.
- Apache Kafka
  - [wurstmeister/kafka](https://hub.docker.com/r/wurstmeister/kafka/)
- Zookeeper
  - [wurstmeister/zookeeper](https://hub.docker.com/r/wurstmeister/zookeeper/)
- zabbix
  - [zabbix/zabbix-server-mysql](https://hub.docker.com/r/zabbix/zabbix-server-mysql/tags/)
  - [zabbix/zabbix-java-gateway](https://hub.docker.com/r/zabbix/zabbix-java-gateway/)
  - [zabbix/zabbix-agent](https://hub.docker.com/r/zabbix/zabbix-agent)
- database
  - [mySQL](https://hub.docker.com/_/mysql)
- grafana
  - [grafana/grafana](https://hub.docker.com/r/grafana/grafana/)

## Install

`docker-compose up`

## Access to zabbix and grafana

- zabbix

  http://localhost:8080
  * Default userID and password is `admin/zabbix`.

- grafana

  http://localhost:3000
  * Default userID and password is `admin/admin`.