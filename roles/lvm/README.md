# lvm

Ansible role for configuring LVM profiles, volume groups and logical volumes.

## Requirements

None.

## Dependencies

None.

## Role Variables

Refer to [defaults/main.yml](defaults/main.yml) for a list of variables along with documentation.

## Example Playbook

```yaml
- hosts: all
  roles:
    - role: hostinger.common.lvm
```

## License

See [LICENSE](../../LICENSE)
