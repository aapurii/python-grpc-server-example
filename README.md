# GRPC echo server example

This is a simple example of grpc echo server with healthcheck and prometheus metrics and client.

# How to build

# Docker

```sh
docker build --platform linux/amd64 -t grpc-server .
docker tag grpc-server <docker_repo_with_tag>
docker push <docker_repo_with_tag>
```

# Locally

Setup prerequisites:

```sh
pip install -r requirements.txt
make proto
```

Run server

```sh
python ./server.py
```

Run client

```sh
python ./client.py
```