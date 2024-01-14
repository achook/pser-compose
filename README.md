# pser-compose

The project relies on https://ants-gitlab.inf.um.es/amzarca/docker-compose-influxdb-grafana, which in turn relies on https://github.com/jkehres/docker-compose-influxdb-grafana to deploy InfluxDB and Grafana. However, the adapter code was added which required changes to the configuration. Also, more default values were added.

## Prerequisites


* Install Docker if they were not previously installed. The instructions can be found on Docker website:
  - [Docker](https://docs.docker.com/engine/install/)
  - [Docker Compose](https://docs.docker.com/compose/install/)
* Deploy the services
```
docker-compose up --build
```
The build flag ensures that the latest version of the code is used.

## Access the default dashboard
 * Go to http://localhost:3000/ and login as user _admin_ with password _admin_ (If you have modified .env, use the new values you have provided)
* Select hamburger menu on the left and select "Dashboards"
* Select "Greenhouse"



## Built With

* [Docker](https://www.docker.com/) - Docker containers
* [influxdb-grafana](https://ants-gitlab.inf.um.es/amzarca/docker-compose-influxdb-grafana) - Base services

## Authors
* Karol Kucza
* Antonio García Serrano

### Based on work of
* Alejandro Molina Zarca

## License

This project is licensed under the MIT License