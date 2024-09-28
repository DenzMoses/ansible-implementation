# ansible-implementation

# Ansible Playbook for Keycloak Realm and Client Creation

This repository contains an Ansible playbook to automate the creation of a Keycloak realm and multiple Keycloak clients. The playbook uses the `community.general` Keycloak modules to manage Keycloak instances and interact with the Keycloak API.

## Playbook Overview

- **Realm Creation**: Automatically creates or updates a Keycloak realm.
- **Client Management**: Configures multiple Keycloak clients (`client-1`, `client-2`, `client-3`) under the specified realm.
- **Delegation**: All tasks are executed on `localhost`, delegating to the local machine running Keycloak.

## Requirements

- **Ansible**: Ensure that Ansible is installed. You can install Ansible via pip: pip install ansible
- **Docker**: Ensure that Docker is installed. You can install Docker by following the steps in here: https://docs.docker.com/engine/install/ubuntu/
- **Keycloak**: Ensure that Keycloak is installed. You can install Keycloak via docker image byr running this command. docker run -p 8080:8080 -e KEYCLOAK_ADMIN=admin -e KEYCLOAK_ADMIN_PASSWORD=admin quay.io/keycloak/keycloak:25.0.6 start-dev


## Steps

Clone the repository : git clone https://github.com/DenzMoses/ansible-implementation.git
Run the command : ansible-playbook playbook.yml


References : 
Keycloak Documentation : https://www.keycloak.org/docs/latest/server_admin/
Ansible Documentation: https://docs.ansible.com/ansible/latest/collections/community/general/keycloak_realm_module.html

