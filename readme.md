##### Create the docker group
`sudo groupadd docker`

##### add user to the docker group
`sudo usermod -aG docker virtualvishal`

##### reload the group
`newgrp docker`

##### To remove all docker containers/images/volumes
`docker system prune -a --volumes`

##### To create image
`docker build -t fastapi-image .`

`docker compose up`

##### To rebuild image
`docker compose up --build -d`

##### To see all docker images
`docker images`

##### To check running docker containers
`docker ps`

##### To run docker container from image
`docker run --name fastapi-container -p 80:80 -d -v $(pwd):/code fastapi-image`

##### To stop running container
`docker stop fastapi-container`

##### To remove container
`docker rm fastapi-container`

##### To delete a specific image
`docker rmi <image_id>`

`docker image rm <image_name>`