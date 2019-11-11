# Prometheus HDFS FSImage Exporter

![Ansible Role](https://img.shields.io/ansible/role/44232?style=flat-square)
![Molecule Test Status](https://img.shields.io/travis/rgibert/ansible-role-prometheus-hdfs-fsimage-exporter?label=molecule&style=flat-square)
![Ansible Quality Score](https://img.shields.io/ansible/quality/44232?style=flat-square)
![Ansible Role](https://img.shields.io/ansible/role/d/44232?label=downloads&style=flat-square)

## Description

Installs a Prometheus exporter for HDFS FSImages

## Requirements

- rgibert.single_binary_service role in roles path

## Role Variables

| Variable | Description |
|----------|-------------|
| prometheus_hdfs_fsimage_exporter_base_url | Base URL for other variables |
| single_binary_service_checksum | SHA256 URL for tarball |
| single_binary_service_dl_url | Tarball download URL |
| single_binary_service_group | Default group for the user to run as |
| single_binary_service_name | Service name |
| single_binary_service_start_cmd | Start command used by service file |
| single_binary_service_stop_cmd | Stop command used by service file |
| single_binary_service_user | User to run the exporter as |
| single_binary_service_version | Version to install |

## Dependencies

- none

## Example Playbook

```yaml
- hosts:
    - servers
  roles:
    - role: rgibert.hdfs_fsimage_exporter
      single_binary_service_version: 1.3
```

## License

GPLv3

## Author Information

Richard Gibert  
[richard@gibert.ca](mailto:richard@gibert.ca)  
[https://richard.gibert.ca/](https://richard.gibert.ca/)
