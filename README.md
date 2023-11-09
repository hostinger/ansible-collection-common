# Hostinger Core Ansible Collection

Collection of Ansible roles for configuring Linux servers used internally at Hostinger.

## Installation

Before using this collection, install it with `ansible-galaxy`:

```bash
ansible-galaxy collection install hostinger.core
```

You can also include it in a `requirements.yml` file:

```yaml
collections:
- name: hostinger.core
```

and install it with:

```bash
ansible-galaxy collection install -r requirements.yml
```

## Usage

To use a role from this collection, prefix it with `hostinger.core`:

```yaml
- hosts: all
  roles:
    - role: hostinger.core.sysctl
      vars:
        sysctl_d: {}
```

## Contributing

Contributions are welcome! For instructions, please refer to the [Contributing](CONTRIBUTING.md) guide.

## License

See [LICENSE](LICENSE).
