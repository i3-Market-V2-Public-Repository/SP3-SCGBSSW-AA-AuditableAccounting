# Auditable Accounting

This repository contains an API that connects to the distributed Storage and Blockchain network from the i3-Market architecture.

* API: Loopback 4
* Database: CockroachDB
* Blockchain: BESU

## Getting started

### Prerequisites

Please make sure you have the following installed and running properly

* [Docker](https://www.docker.com/) and [Docker Compose](https://docs.docker.com/compose/install/)

### Configuration

Edit variables from env.example.

```bash
cp env.example .env
nano .env
```

Then, launch the docker compose to build images and start the container.

```bash
docker compose up -d

```

By default, these are the URLs of each component.

* API: <http://localhost:3000>
* DB Dashboard: <http://localhost:8080>

To access the database exec:

```bash
docker compose exec -it cockroach cockroach sql --insecure

```

## How to build, install, or deploy it

Production procedures are automated with Gitlab CI/CD and AWX. To update deployment, just make a MR to pro branch.

## Credits

Jose Luis Muñoz <jose.luis.munoz@upc.edu>

## Contributing

Pull requests are always appreciated.

## License

EUPL
