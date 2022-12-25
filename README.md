# Proxmox cloud-init tools
ShellScript tools to deploy VM cloud-init in Proxmox Virtual Environment (PVE)
This Script Modified / Update by Nanda Anubis and Testing

### Supported PVE Versions
- PVE 6 *Not tested*
- PVE 7.2 **[OK] - Tested**
- PVE 7.3 **[OK] - Tested**
- Not support local Storage
- LVM-thin **[OK] - Tested**
- ZFS **[OK] - Tested**

### Features
1. Auto cloud images download
- Debian 10 - Buster
- Debian 11 - Bullseye
- Ubuntu Server 20.04 LTS - Focal
- Ubuntu Server 22.04 LTS - Jammy
- Centos 8 
- Centos 9 stream

2. Set VM Hostname
3. Memory (Available to select 2GB,4GB,8GB and 16GB)
4. CPU Cores
5. Storage destination (Local, ZFS, LVM/LVM-Thin, etc)
6. Select bridge network;
7. Select Static/IP or DHCP usage;
8. Define uniq VMID;
9. Can start or not, VM after deployment.

### Usage
1. Login on your Proxmox VE server over SSH or Console Shell
2. Clone proxmox-cloud-init project
```
git clone https://github.com/nandaanubis/deploy-cloudimage-proxmox-v2.git
```
```
cd deploy-cloudimage-proxmox-v2
```
3. Run Sscript 
```
bash deploy.sh
```
4. Follow instructions on screen.

### Contributors
Ananias Filho - @ananiasfilho

Frederico Siena 

## Modified 
Nanda Anubis
