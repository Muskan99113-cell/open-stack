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

"C:\Users\HP\Pictures\M1.0.png"

sunbeam prepare-node-script

sunbeam prepare-node-script | bash -x && newgrp snap_daemon

"C:\Users\HP\Pictures\M2.png"

sunbeam cluster bootstrap --accept-defaults

"C:\Users\HP\Pictures\M3.png"

# CONFIGURE THE CLOUD AND OBTAIN CREDENTIALS
sunbeam configure --accept-defaults --openrc demo-openrc

"C:\Users\HP\Pictures\M1.png"

# LAUNCH VM

sunbeam launch ubuntu --name test
