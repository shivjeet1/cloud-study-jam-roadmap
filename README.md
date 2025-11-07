# Cloud Study Jam Roadmap — Run with Docker

This is a static site for the Cloud Study Jam roadmap. I usually run it locally with Docker so I don’t have to install a web server.

## Prerequisites

- Docker installed
- Git to clone the repo

1) Clone the repo:

```bash
git clone https://github.com/shivjeet1/cloud-study-jam-roadmap.git
cd cloud-study-jam-roadmap
```

2) Build the image:

```bash
docker build -t roadmap:local .
```

3) Run the container from your image:

```bash
docker run -p 8080:80 roadmap:latest
```

Open: http://localhost:8080

## Stop and remove

```bash
docker stop roadmap
docker rm roadmap
```

That’s it. This is the setup I use for local testing using Docker.
