# Compose inside Docker 
This Docker image allows you run Docker and Docker Compose inside a Docker container. This image is generated from Alpine Linux if you prefer use Debian you can use this other image: [composeinsidedocker](https://github.com/irespaldiza/composeinsidedocker). This project has two purposes, on the one hand constitutes a proof of concept and, on the other this is the basis of other of my images, including my development center. If you want to know more about it, follow the following link: walrus.

### How to use this image
 To run this image you have to expose the Docker socket to your Docker CI container, by bind-mounting it with the flag -v.
 ~~~
 docker run -v /var/run/docker.sock:/var/run/docker.sock \   
            -it irespaldiza/composeinsidealpine
~~~
