# Graphite-Grafana-Docker
Graphite + Grafana with docker-compose

## INFO
This setup does not contain SSL configs. If you want to secure communications, please create an nginx proxy or make changes in the configuration. 

## Usage
- Clone repository
- cd /DIR/
- docker-compose up -d
- navigate to Grafana website:
  - http://IP_ADDRESS:3000
  - Use admin:admin to login, than change password
- navigate to Graphite website:
  - http://IP_ADDRESS:81

## Volumes for permanent storage
| Image     | Host Path                     |  Docker Path              |
| -------   | ---------                     | ------------              |
| Grafana   | ./grafana-config              | /etc/grafana/             |
| Grafana   | ./grafana-data                | /var/lib/grafana          |
| Graphite  | ./graphite-storage            | /opt/graphite/storage     |
| Graphite  | ./graphite-config	            | /opt/graphite/conf	|
