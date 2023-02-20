<div align="center">
  
![zabbix_resized](https://user-images.githubusercontent.com/111438070/219988505-c2afa947-c9b3-49c8-ac6c-ee9abc09c707.png)
![docker_resized](https://user-images.githubusercontent.com/111438070/219988579-35fd451e-ca53-4095-aecb-5759d4c8bb1b.png)

</div>

# Zabbix application running via Docker!
I decided to create these files in order to help anyone who needs an easy and fast Zabbix application.
## Summary
The entire structure of the containers was based on the official documentation available on the official [Zabbix website](https://www.zabbix.com/container_images) and the images used are available on the official [Zabbix profile](https://hub.docker.com/u/zabbix) on the Docker Hub.

The basic operating structure is dividing the application into five containers, dividing the application services.
* Zabbix Server
* Zabbix SQL Server
* Zabbix Web
* Zabbix SNMP Trap
* Zabbix agent

In this repository it is possible to find the docker-compose.yml files separated by container, and also a single file for the five containers, facilitating implementation and customization.

## Running the containers
To start the application, you need docker-compose installed in the environment, if you don't have it installed consult the [official Docker documentation](https://docs.docker.com/) on how to install it.

With the environment ready, just copy the file "docker-compose.yml" and run the command *docker-compose up -d*
