# Getting Started

Zuthaka is composed of a front-end that exposes a UI for the API of process manager, file manager, shell post-exploitation modules and general C2 handling, and a back-end, in charge of handling the consistency and availability issues of the C2s instantiated in Zuthaka. Also deployed is [Redis](https://redis.io/) as a message broker to handle asynchronously every element in the Agent's UI and an [Nginx](https://www.nginx.com/) server.

### Prerequisites

The installation of a working [Docker](https://www.docker.com/) instance is necessary for the automatic deployment of the essential infrastructure \(Zuthaka's frontend and backend, Nginx, Redis\). All the desired C2s that need to be handled should be deployed in parallel.

### Docker Installation

To build the full Zuthaka project, first download dependencies.

```bash
 git clone https://github.com/pucara/zuthaka
```

To start the project with the corresponding handler classes, first build the image by running

```bash
docker build .
```

To start the project with the corresponding services, the docker-compose file can be utilized.

```bash
docker-compose up
```

## 

