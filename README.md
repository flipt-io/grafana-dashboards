Flipt Grafana Dashboards
------------------------

This repository contains re-usable Grafana dashboards.
By default, the repository is configured to bootstrap an example Flipt, Postgres, Prometheus and Grafana example setup.

The dashboards, datasources and prometheus are all configured based on this scenario.

## Dependencies

- Docker
- Docker Compose

## Example

Simply run docker-compose to see an example monitoring scenario for Flipt.
The compose setup is configured with a single instance of each of the following:

- Postgres
- Prometheus
- Flipt
- Grafana

```sh
docker-compose up
```

## Installation

The dashboards in the `dashboards/Flipt` folder can be simply imported using Grafanas `import` functionality.
You may need to adjust the name, `uid` and potentially the datasources in your scenario.
This will depend on how and where you configure and run prometheus.
