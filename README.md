## netbeans-ide

[![CI](https://github.com/Oefenweb/ansible-netbeans-ide/workflows/CI/badge.svg)](https://github.com/Oefenweb/ansible-netbeans-ide/actions?query=workflow%3ACI)
[![Ansible Galaxy](http://img.shields.io/badge/ansible--galaxy-netbeans--ide-blue.svg)](https://galaxy.ansible.com/Oefenweb/netbeans_ide)

Set up [NetBeans IDE](https://netbeans.org/features/index.html) in Debian-like systems.

#### Requirements

None

#### Variables

* `netbeans_ide_assume_java_provided` [default: `false`]: Whether or not to assume that java (`jre` and `jdk`) is already installed

* `netbeans_ide_version` [default: `13`]: Version to install
* `netbeans_ide_state_file` [optional, default `files/state.xml`]: State file to use for installation

## Dependencies

None

## Recommended

* `ansible-oracle-java` ([see](https://github.com/Oefenweb/ansible-oracle-java), when `netbeans_ide_assume_java_provided` is `true`)

#### Example

```yaml
---
- hosts: all
  roles:
    - netbeans-ide
```

#### License

MIT

#### Author Information

Mischa ter Smitten

#### Feedback, bug-reports, requests, ...

Are [welcome](https://github.com/Oefenweb/ansible-netbeans-ide/issues)!
