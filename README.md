# Ansible Role: WireGuard

An Ansible Role that installs and configures [WireGuard](https://www.wireguard.com/).

## Requirements

None.

## Role Variables

See [Example Playbook](#example-playbook) section.

## Dependencies

None.

## Example Playbook

```
---
- hosts: localhost
  roles:
    - role: galaxy-wireguard
      address: <ip>
      private_key: <private_key>
      listen_port: 21841
      persistant_keepalive: 25
      peers:
        - public_key: <public_key>
          endpoint: <endpoint>
          allowed_ips: <allowed_ips>
```

## License

GPLv3

## Author Information

This role is developed and maintained by [Sven Kube](https://github.com/svenkube)
