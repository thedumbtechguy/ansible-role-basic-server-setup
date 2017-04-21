# Ansible Role: server_setup

An ansible role to configure some basics on a new linux host.

## Requirements

> This role has been tested on `Ubuntu 16.04` and `Ubuntu 16.10` only.

## Configuration Actions

### Network

Set the hostname and disable ipv6.

#### Variables

- `network_server_fqdn`: the hostname to set for this host.
  - Default: `[undefined]`
  > **NOTE**:  this should be set per host, ideally as an inventory variable.

- `network_disable_ipv6`: disable ipv6.
  - Default: `false`

### SSH

Configure SSH to use a centralized authorized_keys location for easy management.


## Usage Example

```yaml
- hosts: all
  roles:
    - thedumbtechguy.server-setup
```


## License

MIT / BSD

## Author Information

This role was created by [Stefan Froelich](https://thedumbtechguy.blogspot.com/).

## Credits