# How to launch docker in GUI mode
* This repository is to provide the command and the Dockerfile to launch an application in docker container in GUI mode. 
* > To know more in details please follow this [article]()
* The command used to run is `docker run -e DISPLAY -v /home/root/.Xauthority:/root/.Xauthority   --net=host <app_name>`
* Where :
* - `-e DISPLAY` : We will pass the DISPLAY environment variable of our host OS to the container.
* - `-v /root/.Xauthority:/root/.Xauthority` : will attach the volume of the X server which is in /root/.Xauthority to the container.
*  - `--net=host` : will specify the network we're going to use in our container.
