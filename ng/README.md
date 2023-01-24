## docker 
- Run `docker pull nginx` to get an nginx image from Docker Hub if you don't have one locally
- Run `docker run -it --rm -d -p 8080:80 --name Ngnix_demo nginx` make a new container and run with the ngnix image with the name 'Ngnix_demo'
- Run `docker build -t webserver_nginx .` to build a custom image
- Run `docker run -it --rm -d -p 8080:80 --name nginx_web_server webserver_nginx` to make a container with the custom image
- Run `docker top <container_name>` to see running processes
- Run `docker-compose build` to build a container from the yaml file

## ngnix commands
- Run `server nginx start` to stop nginx and its container
- Run `server nginx stop` to stop nginx and its container
- Run `nginx -v` or `nginx -V` for verbose  to see nginx version
- Run `nginx -t` or `nginx -T` for verbose  to see nginx's configuration or html file location
- Run `nginx -s signal` to send a signal to the nginx server exp `nginx -s stop` to stop the server or Run `nginx -s reload` to reload the nginx server


## yaml file description
- 
