# Dockerized Static Website with Nginx

This repository contains a static website deployed using Docker and Nginx. The setup leverages Docker Compose to orchestrate the containerized web server and host configuration. It’s a production-style implementation of serving HTML/CSS content via an optimized Nginx container.

---

##  Features

-  Dockerized deployment of static HTML website
-  Custom Nginx configuration for routing
-  Organized folder structure for maintainability
-  Easy to run locally with Docker Compose

---

##  Project Structure

```
.
├── docker-compose.yml          # Compose configuration
├── nginx/
│   └── default.conf            # Custom Nginx configuration
└── website/
    ├── index.html              # Main homepage
    ├── jewellary.html          # Jewelry category
    ├── footwear.html           # Footwear category
    ├── outfit.html             # Outfit category
    └── *.jpg                   # Image assets
```

---

## Getting Started

### Prerequisites

- [Docker Engine](https://docs.docker.com/engine/install/)
- [Docker Compose](https://docs.docker.com/compose/install/)

### Steps to Run

1. Clone the repository:

```bash
git clone https://github.com/your-username/docker-nginx-website.git
cd docker-nginx-website
```

2. Build and start the application:

```bash
docker compose up --build
```

3. Open your browser and visit:

```
http://localhost:8080
```

---

##  How It Works

- Docker Compose builds the Nginx container.
- Website files from `./website` are mounted as static assets.
- Nginx uses the provided `default.conf` to serve HTML content from `/usr/share/nginx/html`.
- The container maps port `8080` on the host to port `80` inside the container.

---

## Website Pages

- `index.html` – Homepage
- `jewellary.html` – Jewelry category
- `footwear.html` – Footwear category
- `outfit.html` – Outfit category

---

## Clean Up

To stop and remove the containers:

```bash
docker-compose down
```

“This website was originally a fun project I built during my college days. While learning Docker, I decided to revisit it and containerize the application using Docker and Nginx. It turned out to be a great hands-on experience, combining nostalgia with practical learning.”


