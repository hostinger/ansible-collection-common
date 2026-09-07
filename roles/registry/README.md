# registry

Ansible role to install and configure [distribution/registry](https://github.com/distribution/distribution).

## Requirements

None.

## Dependencies

None.

## Role Variables

Refer to [defaults/main.yml](defaults/main.yml) for a list of variables along with documentation.

## Example Playbook

Each instance of the role manages one registry, named by `registry_name`, and
owns `/etc/registry/<registry_name>.yml` and
`/etc/systemd/system/registry-<registry_name>.service`. Nothing is shared
between instances, so the role can be used several times on one host:

```yaml
- hosts: all
  roles:
    - role: hostinger.common.registry
      vars:
        registry_name: cache
        registry_config: "{{ registry_config_cache }}"
    - role: hostinger.common.registry
      vars:
        registry_name: docker.io
        registry_config: "{{ registry_config_docker_io }}"
```

Registries used to run from a shared `registry@.service` template unit. Hosts
that still have it need the old units stopped and disabled before the new ones
can bind their addresses.

## License

See [LICENSE](../../LICENSE)
