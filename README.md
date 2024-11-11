# Project URL
https://roadmap.sh/projects/configuration-management

# Ansible Configuration Management Project

This repository contains an Ansible playbook for configuring a Linux server with the following roles:

1. **base**: Basic server setup (installs utilities, updates the server, installs fail2ban, etc.)
2. **nginx**: Installs and configures NGINX.
3. **app**: Uploads the given tarball of a static HTML website to the server and unzips it.
4. **ssh**: Adds the given public key to the server.

## Prerequisites

Before running the playbook, ensure you have the following:

1. A Linux server (e.g., an EC2 instance) running Ubuntu.
2. Ansible installed on your local machine. You can install it by running:

    ```bash
    sudo apt update
    sudo apt install ansible -y
    ```

3. SSH access to your server and the server’s public IP.

4. A `tar.gz` file for the website (if needed for the app role).
