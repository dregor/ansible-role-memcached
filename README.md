# Ansible Role: Memcached

Installs Memcached (latest)

## Supported platforms

```
CentOS 6 & 7
Ubuntu 14.04
```

## Requirements

None

## Role Variables

Start:

```
memcached_start: true
```

Start on boot:

```
memcached_start_on_boot: true
```

Listen address:

```
memcached_address: 127.0.0.1
```

Listen port:

```
memcached_port: 11211
```

Memory:

```
memcached_memory: 64
```

Max connections:

```
memcached_connections: 1024
```

## Dependencies

```
pcextreme.repo-epel
pcextreme.repo-pcextreme
```

## Example Playbook

```
- hosts: servers
  roles:
    - { role: pcextreme.memcached }
```

## Credits

- [Attila van der Velde](https://github.com/vdvm)

## License

The MIT License (MIT). Please see [License File](LICENSE) for more information.
