# Ansible Role: Cumulus upgrade


## Heavily inspired/copied from Eric Pulvino.

This role will prepare and start the upgrade of switches, taking care of ospf and/or clag failover.

Naturalis uses this role together with a private inventory.

## Requirements

None.

## Role Variables

Available variables are listed below.
```bash
desired_image: https://192.168.0.254/cumulus-linux-3.7.0-bcm-amd64.bin
ztp_url: http://192.168.144.5/ztp_oob.sh
counter_threshold: 1000
```

## Dependencies

None.

## Example Playbook
```bash
    - hosts: switches
      roles:
        - ansible-cumulus-upgrade
```
## License

Apache2
