# Bakery App

A simple, beautiful bakery website containerized with Docker.

## Features

- Single-page web application with a bakery theme
- Responsive design that works on desktop and mobile
- Containerized using Docker for easy deployment
- Served with nginx for optimal performance

## Prerequisites

- Docker installed on your system
- (Optional) Docker Compose

## Quick Start

### Building the Docker Image

```bash
docker build -t bakery-app .
```

### Running the Container

```bash
docker run -d -p 8080:80 --name bakery-app bakery-app
```

The application will be available at `http://localhost:8080`

### Stopping the Container

```bash
docker stop bakery-app
docker rm bakery-app
```

## Project Structure

```
bakery-app/
├── index.html      # Main HTML page
├── styles.css      # CSS styling
├── Dockerfile      # Docker configuration
├── nginx.conf      # Nginx server configuration
├── .dockerignore   # Docker ignore file
└── README.md       # This file
```

## Development

To make changes to the website:

1. Edit `index.html` or `styles.css`
2. Rebuild the Docker image: `docker build -t bakery-app .`
3. Restart the container with the new image

## Technologies Used

- HTML5
- CSS3
- Docker
- Nginx (Alpine Linux)