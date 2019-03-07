# Ansible Role: Cumulus upgrade


* Heavily inspired by [Eric Pulvino](https://github.com/CumulusNetworks/upgrade_playbook/blob/master/dataplane_upgrade_playbook.yml).

This role will prepare and start the upgrade of switches, taking care of ospf and/or clag failover.
Naturalis uses this role together with a private inventory.

## Requirements

None.

## Role Variables

Available variables are listed below.
```bash
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
