# Portainer Automation

This repository contains an Ansible playbook to set up Portainer on a Proxmox VM.

## Files

- `ansible/setup_portainer.yaml`: Ansible playbook to install and configure Portainer.

## Prerequisites

- Ansible installed on your local machine.
- Proxmox VM set up and accessible.

## Usage

1. Clone this repository:
    ```sh
    git clone https://github.com/18visions/portainer_automation.git
    cd portainer_automation
    ```

2. Run the Ansible playbook:
    ```sh
    ansible-playbook ansible/setup_portainer.yaml
    ```

## Playbook Details

The playbook performs the following tasks:
1. Installs required dependencies.
2. Adds Docker GPG key and repository.
3. Installs Docker and its dependencies.
4. Enables and starts Docker service.
5. Ensures Python Docker SDK is installed.
6. Creates Portainer data directory.
7. Deploys Portainer container.
8. Verifies Portainer is running and displays its status.

Access Portainer at `https://<your-ip-address>:9443`.

## License

This project is licensed under the MIT License.
