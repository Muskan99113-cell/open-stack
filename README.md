# OPEN STACK
# REQUIREMENTS
You will need a single machine whose requirements are:

1. physical or virtual machine running Ubuntu 22.04 LTS
2. a multi-core amd64 processor ideally with 4+ cores
3. a minimum of 16 GiB of free memory
4. 50 GiB of SSD storage available on the root disk
# Deploy the cloud
Install the openstack snap---
sudo snap install openstack --channel 2024.1/beta

![M1 0](https://github.com/user-attachments/assets/709b097f-10b6-49be-875d-94faa6012ddd)


sunbeam prepare-node-script

sunbeam prepare-node-script | bash -x && newgrp snap_daemon

sunbeam cluster bootstrap --accept-defaults

![M3](https://github.com/user-attachments/assets/d1e76773-65ad-423d-9ca0-f716da54000c)

"

# CONFIGURE THE CLOUD AND OBTAIN CREDENTIALS
sunbeam configure --accept-defaults --openrc demo-openrc

![M1](https://github.com/user-attachments/assets/7b8f50e4-0de7-4884-804e-7e73d3f28ea4)


# LAUNCH VM

sunbeam launch ubuntu --name test
