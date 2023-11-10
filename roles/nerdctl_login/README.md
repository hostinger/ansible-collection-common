# nerdctl_login

Ansible role for logging into container registries using [nerdctl](https://github.com/containerd/nerdctl).

## Requirements

The nerdctl binary must be installed on the target host and available in the PATH before running this role. This can be done by using the [hostinger.core.nerdctl](../nerdctl) role.

The [jmespath](https://pypi.org/project/jmespath/) Python package must be installed on the source host before running this role.

## Dependencies

None.

## Role Variables

Refer to [defaults/main.yml](defaults/main.yml) for a list of variables along with documentation.

## Example Playbook

```yaml
- hosts: all
  roles:
    - role: hostinger.core.nerdctl_login
```

## License

See [LICENSE](../../LICENSE)
