
#### To list available network 

```
docker network ls
```
#### To create network
```
docker network create -d bridge network name

--driver , -d	bridge	Driver to manage the Network
```
#### To create network with gatweay, subnetmask options 
```
 docker network create \
  --driver=bridge \
  --subnet=182.18.0.1/24 \
  --gateway=182.18.0.1 \
 wp_mysq-network
 ```
 #### To run a container with mysql image , settings enviromental varaiable and assigning to a network
 
 ```
 docker container run --name mysql-db -e MYSQL_ROOT_PASSWORD=db_pass123 -d --network=wp-mysql-network mysql:5.6
 ```
 
 





            

            .
           





