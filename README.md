# Python 
## Virtual Environment
### Create
```
python -m venv NmaeofVirtualEnv
```
### Activate it 
``` 
source path/to/virtualemvironment/bin/activate
```
### Create requirement.txt
```
pip freeze > requirements.txt
```
### Install using requirements.txt
```
pip install -r requirements.txt
```

# Linux Commands 
## Pacman
### See Installed Packages
```
pacman -Q
```
#### List Foreign (Manually Installed or AUR) Packages:

```
pacman -Qm
```
#### List packages by installation date:
```
pacman -Qi | grep -E "Name|Install Date" | paste - - | sort -k4,5
```
### remove lock file 
##### :: Synchronizing package databases...
##### error: failed to synchronize all databases (unable to lock database)
```
sudo rm /var/lib/pacman/db.lck

```
# Docker
## Docker pull

```
#if you dont specify the version then its gonna pull the latest
docker pull name:version
```
