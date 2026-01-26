# Ansible  k3s cluster
Ansible scripts to create a k3s cluster.  
WIP - moved from the gitops repo.

## Usage

### Setup ansible
```bash
# Create virtual environment
python3 -m venv .venv
source .venv/bin/activate

# Install ansible
python -m pip install ansible
ansible-galaxy collection install community.general kubernetes.core
```

### Run

```bash
# Activate virtual environment
source .venv/bin/activate

# Run ansible
ansible-playbook ansible/k3s-cluster/main.yaml -i home-k8s/ansible-inventory.yaml
```