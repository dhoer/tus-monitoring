# Zabbix Monitoring

## Requirements

Setup a Zabbix server and NGINX and configure monitoring for the following parameters on main dashboard:

1. CPU
1. Memory
1. Network Bandwidth
1. Storage

## Prerequisites

- Docker
- Docker Compose


## Executing

Create and start containers in background:

    docker-compose up -d
    
Login to https://localhost:8080 as Admin/zabbix and navigate to dashboard


Load test nginx:

    ab -n 30000 http://localhost:8088/
 
Stop and remove containers, networks, images, and volumes:

    docker-compose down
 