# Traefik Demo

## How to run
### Bring up traefik
    ```
    docker-compose up -d reverse-proxy
    ```

    Navigate to http://localhost:8080/api/rawdata => To see the Trafik's API raw data
    
    Navigate to http://localhost:8080/dashboard/#/ => To see Trafik's Dashboard

### Bring up a service

    docker-compose up whoami

    Navigate to => http://whoami.docker.localhost/

### Load balacing

    docker-compose up -d --scale whoami=2 => Increase instances