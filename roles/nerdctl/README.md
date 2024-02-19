# nerdctl

Ansible role to install and configure [nerdctl](https://github.com/containerd/nerdctl).

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
    - role: hostinger.common.nerdctl
```

## License

See [LICENSE](../../LICENSE)
