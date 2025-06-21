Chess Gif Generator from Lichess.org
==========

Golang application that converts any Lichess game to an animated GIF with a modern web interface. 

Try it out at https://gif.chesstools.org/. 

![example gif](assets/example.gif)

## Features

- **Web Interface**: User-friendly HTML form for easy GIF generation
- **Board Flipping**: Option to view games from Black's perspective
- **Responsive Design**: Works on desktop and mobile devices
- **Fast Processing**: Optimized for quick GIF generation
- **Docker Ready**: Containerized for easy deployment
- **Heroku Compatible**: Deploy to Heroku with one command
- **API Endpoints**: RESTful API for programmatic access

## Live Demo

- **Web Interface**: Access the modern web UI at your deployed instance
- **API Access**: Use RESTful endpoints for integration

## Table Of Contents
1. [Installation](#installation)
2. [Usage](#usage)
   - [Web Interface](#1-web-interface)
   - [API Usage](#2-api-usage)
   - [CLI Usage](#3-cli-usage)
   - [Server Usage](#4-server-usage)
3. [Deployment](#deployment)
4. [Development](#development)
5. [API Reference](#api-reference)

## Installation

### Using Docker (recommended)

```bash
# Build for production
docker build -t giflichess:latest .

# Run in production
docker run -d -p 8080:8080 --name giflichess-prod giflichess:latest serve

# Or with docker-compose
docker-compose up -d
```

### Heroku Deployment

This application is configured for easy Heroku deployment using `heroku.yml`:

1. **Prerequisites:**
   ```bash
   # Install Heroku CLI
   # Login to Heroku
   heroku login
   ```

2. **Deploy:**
   ```bash
   # Create Heroku app (if not exists)
   heroku create your-app-name
   
   # Deploy using Git
   git push heroku main
   
   # Open your deployed app
   heroku open
   ```

3. **View logs:**
   ```bash
   heroku logs --tail
   ```
