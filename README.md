# centos-common (ansible role)

This role intends to provide command setup routine for CentOS.

## Requirements

This role requires Ansible 1.2 or higher, and platform requirements are listed in the metadata file.

## Role Variables

see `defaults/main.yml`.

You're encouraged to override repo settings like

```
common_repos:
  - name: base
    description: CentOS-$releasever - Base
    baseurl: http://your.yum.repo/centos/$releasever/os/$basearch/
    enabled: 1
    gpgcheck: 0
    gpgkey: ""
  - name: updates
    description: CentOS-$releasever - Updates
    baseurl: http://your.yum.repo/centos/$releasever/updates/$basearch/
    enabled: 1
    gpgcheck: 0
    gpgkey: ""
  - name: extras
    description: CentOS-$releasever - Extras
    baseurl: http://your.yum.repo/centos/$releasever/extras/$basearch/
    enabled: 1
    gpgcheck: 0
    gpgkey: ""
```

## Dependencies

None

## License

MIT

## Author Information

AR <aleiphoenix@gmail.com>
