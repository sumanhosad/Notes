# Python 
## Virtual Environment
### Create
```bash
python -m venv NmaeofVirtualEnv
```
### Activate it 
``` bassh
source path/to/virtualemvironment/bin/activate
```
### Create requirement.txt
```bash
pip freeze > requirements.txt
```
### Install using requirements.txt
```bash
pip install -r requirements.txt
```

# Linux Commands 
## Pacman
### See Installed Packages
```bash
pacman -Q
```
#### List Foreign (Manually Installed or AUR) Packages:

```bash
pacman -Qm
```
#### List packages by installation date:
```bash
pacman -Qi | grep -E "Name|Install Date" | paste - - | sort -k4,5
```
### remove lock file 
- :: Synchronizing package databases...
- error: failed to synchronize all databases (unable to lock database)
```bash
sudo rm /var/lib/pacman/db.lck

```
# Docker

## Docker pull
if you dont specify the version then its gonna pull the latest
```bash
docker pull name:version
```

## Docker run

To run a basic container using an image, use the following command:
```bash
docker run <image_name>
```
To start a container and access its interactive shell:
```bash
docker run -it <image_name>
```
To run a container in the background (detached mode):
```bash
docker run -d <image_name>
```
To assign a specific name to the container:
```bash
docker run --name <container_name> -it <image_name>
```
To expose a port from the container to the host:
```bash
docker run -p <host_port>:<container_port> -d <image_name>
```

## Docker stop

List Running Containers
```bash
docker ps
```
List All Containers
```bash
docker ps -a
```
Stop The Running Container
```bash
docker stop <container_id_or_name>
```

## Docker Registries

### A Docker registry is a service for storing and distributing Docker images.

Log In to a Docker Registry
```bash
docker login <registry_url>
```
Log Out from a Docker Registry
```bash
docker logout <registry_url>
```
To download an image from a registry
```bash
docker pull <image_name>:<version/tag>
```
To upload an image to a registry
```bash
docker push <image_name>:<tag>
```
Search for Images in a Registry
```bash
docker search <search_term>
```
List Local Images
```bash
docker images
```
To delete an image from your local registry
```bash
docker rmi <image_name>:<tag>
```
