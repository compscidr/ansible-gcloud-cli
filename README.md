# ansible-gcloud-cli
Ansible collection to install Google Cloud CLI (gcloud) tool

## Installation

Install this collection using ansible-galaxy:

```bash
ansible-galaxy collection install compscidr.gcloud_cli
```

## Usage

### Using the role in a playbook

```yaml
- name: Install Google Cloud CLI
  hosts: all
  roles:
    - compscidr.gcloud_cli.gcloud_cli
```

### Using the example playbook

```bash
ansible-playbook -i inventory playbook.yml
```

## Requirements

- Ubuntu 18.04+ or Debian 10+
- Ansible 2.15+
- sudo privileges

## What it does

This collection installs the Google Cloud CLI by:

1. Installing prerequisites (apt-transport-https, ca-certificates, gnupg, curl)
2. Importing the Google Cloud GPG key
3. Adding the Google Cloud SDK repository
4. Installing the google-cloud-sdk package

## Tags

All tasks are tagged with `gcloud_cli` so you can run specific parts:

```bash
ansible-playbook playbook.yml --tags gcloud_cli
```

## License

GPLv3
