# Nginx Static Web Server

This project is a simple static web server using [Nginx](https://www.nginx.com/) and [Docker Compose](https://docs.docker.com/compose/). Static HTML files are served from the `src` folder.


## How to Run

1. **Make sure Docker and Docker Compose are installed on your system.**

2. **Start the server using:**
   ```sh
   docker-compose up -d

3. **Access the website**
   Open your browser and go to 
   http://localhost

## EXPLANATION
   - **docker-compose.yml**
    Uses the nginx:latest image and maps port 80 on the host to port 80 in the container. The src folder is mounted to /usr/share/nginx/html inside the container, so all static files in src are served by Nginx.
   - **src/index.html**
     The static HTML file displayed in the browser.

## Stopping the Server
To Stop and remove the container:
```bash
   docker-compose down
