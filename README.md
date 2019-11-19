# Prometheus HDFS FSImage Exporter

![Ansible Role](https://img.shields.io/ansible/role/44536?style=flat-square)
![Molecule Test Status](https://img.shields.io/travis/rgibert/ansible-role-prometheus-hdfs-fsimage-exporter?label=molecule&style=flat-square)
![Ansible Quality Score](https://img.shields.io/ansible/quality/44536?style=flat-square)
![Ansible Role](https://img.shields.io/ansible/role/d/44536?label=downloads&style=flat-square)

## Description

Installs a Prometheus exporter for HDFS FSImages

## Requirements

- rgibert.single_binary_service role in roles path

## Role Variables

| Variable | Description |
|----------|-------------|
| prometheus_hdfs_fsimage_exporter_base_url | Base URL for other variables |
| prometheus_hdfs_fsimage_exporter_checksum | SHA256 URL for tarball |
| prometheus_hdfs_fsimage_exporter_dl_url | Tarball download URL |
| prometheus_hdfs_fsimage_exporter_group | Default group for the user to run as |
| prometheus_hdfs_fsimage_exporter_user | User to run the exporter as |
| prometheus_hdfs_fsimage_exporter_version | Version to install |
| prometheus_hdfs_fsimage_exporter_max_heap | Max heap allocated to the exporter |
| prometheus_hdfs_fsimage_exporter_ip | IP to listen on |
| prometheus_hdfs_fsimage_exporter_port | Port to listen on |
| prometheus_hdfs_fsimage_exporter_conf_path | Path to the config file |
| prometheus_hdfs_fsimage_exporter_conf_file | Config file |
| prometheus_hdfs_fsimage_exporter_fsimage_path | Path the HDFS fsimage |
| prometheus_hdfs_fsimage_exporter_skip_file_distrib_for_group_stats | Skip file size distribution for group based stats |
| prometheus_hdfs_fsimage_exporter_skip_file_distrib_for_user_stats | Skip file size distribution for user based stats |
| prometheus_hdfs_fsimage_exporter_paths | Paths to track stats for |
| prometheus_hdfs_fsimage_exporter_skip_file_distrib_for_path_stats | Skip file size distribution for path based stats |
| prometheus_hdfs_fsimage_exporter_path_sets | Sets for grouping paths |
| prometheus_hdfs_fsimage_exporter_skip_file_distrib_for_path_set_stats | Skip file size distribution for path set based stats |
| prometheus_hdfs_fsimage_exporter_file_size_buckets |  |


## Dependencies

- none

## Example Playbook

```yaml
- hosts:
    - servers
  roles:
    - role: rgibert.hdfs_fsimage_exporter
      prometheus_hdfs_fsimage_exporter_version: 1.3
```

## License

GPLv3

## Author Information

Richard Gibert  
[richard@gibert.ca](mailto:richard@gibert.ca)  
[https://richard.gibert.ca/](https://richard.gibert.ca/)
