## Docker Imageing Steps.

Pre-req:
-> Create a docker hub account & we are going to use that account in making images.
Assume your account name is `vamsic999` then all the images comes as `vamsic999/image-name:tag`

Pre-Steps:

Login to Docker Account over Cli

`docker login`


1. Write a Dockerfile.


2. Build the Image from Dockerfile. `vamsic999/<image-name>:tag`
docker build -t `vamsic999/image-name:tag` .


3. Push the image centrally
docker push `vamsic999/image-name:tag`