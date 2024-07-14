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

```bash
#if you dont specify the version then its gonna pull the latest
docker pull name:version
```
### Docker run


```bash
docker run <image_name>
