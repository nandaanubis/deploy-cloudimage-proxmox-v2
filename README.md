# Proxmox cloud-init tools
ShellScript tools to deploy VM cloud-init in Proxmox Virtual Environment (PVE)
This Script Modified / Update by Nanda Anubis and Testing

### Supported PVE Versions
- PVE 6 *Not tested*
- PVE 7.2 **[OK] - Tested**
- PVE 7.3 **[OK] - Tested**

### Features
1. Auto cloud images download
- Debian 9 - Stretch
- Debian 10 - Buster
- Ubuntu Server 18.04 LTS - Bionic
- Ubuntu Server 20.04 LTS - Focal
- OpenSUSE LEAP 15.2
2. Set VM Hostname
3. Memory (Available to select 2GB,4GB,8GB and 16GB)
4. CPU Cores
5. Storage destination (Local, NFS, LVM/LVM-Thin, etc)
6. Select bridge network;
7. Select Static/IP or DHCP usage;
8. Define uniq VMID;
9. Can start or not, VM after deployment.

### Usage
1. Login on your Proxmox VE server over SSH or Console Shell
2. Clone proxmox-cloud-init project
```
git clone https://github.com/kmee/proxmox-cloud-init-tools.git
```
```
cd proxmox-cloud-init-tools
```
3. Create authorized keys files
```
mkdir pub_keys
```
```
touch pub_keys/id_rsa.pub
```
**copy your public ssh keys to pub/keys/id_rsa.pub file**

4. Adjust permission, then run deploy.sh
```
chmod +x deploy.sh
```
```
./deploy.sh
```
5. Follow instructions on screen.

### Important
Before deploy VM using things script, upload your public ssh key to ./pub_keys/id_rsa.pub file.
if you do not upload keys do pub_keys/id_rsa.pub, you will not access VM.

### Contributors
Ananias Filho - @ananiasfilho

Frederico Siena 
