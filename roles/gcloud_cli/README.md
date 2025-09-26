# Google Cloud CLI Ansible Role

This role installs the Google Cloud CLI (gcloud) on Ubuntu and Debian systems.

## Requirements

- Ubuntu 18.04+ or Debian 10+
- Ansible 2.4+
- sudo privileges

## Role Variables

This role does not require any variables.

## Dependencies

None.

## Example Playbook

```yaml
- hosts: servers
  roles:
    - compscidr.gcloud_cli.gcloud_cli
```

## License

GPLv3

## Author Information

Jason Ernst <ernstjason1@gmail.com>