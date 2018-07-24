## Prometheus Monitoring

This repository contains minimal Prometheus Server, NodeExporter, BlackBoxExporter, AlertManager and Grafana implementation for monitoring various services. You can use this repository to monitor a bare-metal Linux instance or to monitor Apache, NGINX or other HTTP based service using Prometheus.

## Monitoring a Bare-Metal Linux Server

To monitor a stand-alone Linux Server, you need to uncomment the `nodeexporter` service in the `docker-compose.yml` file and configure AlertManager accordingly.

## Monitoring HTTP-based Web Services

This repo 2 HTTP-based Web Services by default: An Apache httpd server and NGINX server both running in Docker Containers. If either or both of them goes down, an Prometheus Will fire an Alert in the form emails specified in the `config.yml` file in the AlertManager folder.