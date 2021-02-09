# How to deploy

## Make sure your Ubuntu version is 20.04 or above

## Install Multipass client

```
sudo apt-get update
sudo apt-get upgrade -y
sudo snap install multipass --classic --stable
```

## Configure VM informations
### Names, number of workers
master="master"
slaves="worker-1 worker-2"
vms=$master" "$slaves

### Master resources
master_cpus=2
master_mem=4G
master_disk=15G

### Worker resourses
slaves_cpus=1
slaves_mem="2G"
slaves_disk="10G"

## Start script
```
bash deploy-k3s-ubuntu.sh
```
