docker-statsd-influxdb
======================

Out-of-the-box StatsD + InfluxDB backend image for Docker


## Running

Example command to run this image:

    docker run -p 8125:8125 -e "INFLUXDB_HOST=localhost" -e "INFLUXDB_DATABASE=site_dev" -e "INFLUXDB_USERNAME=username" -e "INFLUXDB_PASSWORD=password" -e "STATSD_DEBUG=true" shakr/statsd-influxdb

Following environment varaiables can be used:

- `INFLUXDB_HOST` (default: localhost)
- `INFLUXDB_PORT` (default: 8086)
- `INFLUXDB_DATABASE` (default: site_dev)
- `INFLUXDB_USERNAME` (default: root)
- `INFLUXDB_PASSWORD` (default: root)
- `STATSD_PORT` (default: 8125)
- `STATSD_DEBUG` (default: false)