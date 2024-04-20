# k8s on ARM64

This repository contains the Vagrantfile and [Kubernetes CKS Course Environment](https://github.com/killer-sh/cks-course-environment) scripts to create a Kubernetes cluster on ARM64 using [Vagrant Parallels Provider](https://github.com/Parallels/vagrant-parallels).

## Vagrant Commands

```bash
# Start the VMs
vagrant up

# SSH into the VMs
vagrant ssh control-plane
vagrant ssh node1
vagrant ssh control-plane -c "cat /etc/*release"

# Stop the VMs
vagrant halt
vagrant halt control-plane

# Destroy the VMs
vagrant destroy -f
vagrant destroy control-plane -f
```