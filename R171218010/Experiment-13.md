# Experiment 13: Docker basic commands.

## Steps Performed

- ```docker images```: List docker images present in system.
![Screenshot from 2020-11-27 02-21-54](https://user-images.githubusercontent.com/46739435/100390701-5453d400-3057-11eb-8860-ab962ff5a180.png)

- ```docker search```: Search the Docker Hub for images.
![Screenshot from 2020-11-27 02-23-11](https://user-images.githubusercontent.com/46739435/100390754-82391880-3057-11eb-9120-97a9c3686bf4.png)

- ```docker pull```: Pull an image or a repository from a registry.
![Screenshot from 2020-11-27 02-26-36](https://user-images.githubusercontent.com/46739435/100390937-fd023380-3057-11eb-8aee-ae6f3c9f17bc.png)

- ```docker ps```: List containers.             
![Screenshot from 2020-11-20 12-09-36](https://user-images.githubusercontent.com/46739435/100391087-67b36f00-3058-11eb-901d-7b3df436b2d9.png)

- ```docker run```: Run a command in a new container.
![Screenshot from 2020-11-20 12-02-47](https://user-images.githubusercontent.com/46739435/100391175-a3e6cf80-3058-11eb-8976-5d381852a4b3.png)

- ```docker start```: Start one or more stopped containers
![Screenshot from 2020-11-27 02-42-34](https://user-images.githubusercontent.com/46739435/100391693-45225580-305a-11eb-8eba-697e2a756285.png)

- ```docker stop```: Stop one or more running containers.
![Screenshot from 2020-11-27 02-33-55](https://user-images.githubusercontent.com/46739435/100391310-0213b280-3059-11eb-86a4-e79af32cb94a.png)

- ```docker ps -a```: List all containers.
![Screenshot from 2020-11-27 02-35-15](https://user-images.githubusercontent.com/46739435/100391371-338c7e00-3059-11eb-935d-f7ce6b2a5a2b.png)

- ```docker run -it ubuntuNetwork -p 81:81 ubuntu```
  -i, --interactive                    Keep STDIN open even if not attached
  -p, --publish list                   Publish a container's port(s) to
                                       the host
  -t, --tty                            Allocate a pseudo-TTY
![Screenshot from 2020-11-20 12-11-25](https://user-images.githubusercontent.com/46739435/100391532-bf060f00-3059-11eb-9f60-3fd0fd565bb0.png)
![Screenshot from 2020-11-20 12-04-50](https://user-images.githubusercontent.com/46739435/100391611-faa0d900-3059-11eb-8200-d840173e86e9.png)

- ```docker inspect```: Return low-level information on Docker objects
![Screenshot from 2020-11-20 12-09-16](https://user-images.githubusercontent.com/46739435/100391604-f83e7f00-3059-11eb-8038-646492f7d5e9.png)

