# Ansible Role: Java

[![Build Status](https://travis-ci.org/T2L/ansible-role-java.svg?branch=1.0.0)](https://travis-ci.org/T2L/ansible-role-java)

Installs Java on Ubuntu LTS using [OpenJDK builds PPA](https://launchpad.net/~openjdk-r/+archive/ubuntu/ppa) and/or [Oracle Java (JDK) 8/9 Installer PPA](https://launchpad.net/~webupd8team/+archive/ubuntu/java).

## What is so special about this Java role

- No need to know actual package name(s). Just follow the instructions below
- One role to install OpenJDK and Oracle Java at the same time (if configured)
- Supports Ubuntu 14.04 and 16.04 only
- Testing with [Molecule](https://github.com/metacloud/molecule)

## Requirements

None.

## Role Variables

Available variables are listed below, along with examples values (see [defaults/main.yml](defaults/main.yml)):

OpenJDK versions and types to install. OpenJDK currently supports installing JDK 6, 7 and 8. Also, it's possible to install JRE or JDK:

    java_openjdk_packages:
      - version: 8
        type: jre

Oracle Java versions to install. Oracle Java supports installing JDK 8 and 9. It's not possible to select package type. Only the **version** key is supported, possible values are 8 and 9.

    java_oracle_packages: []


Example (do not forget to remove square brackets):

    java_oracle_packages:
      - version: 8

Default Java to use. Also affects JAVA_HOME environment variable (will be pointing to the same location). Possible keys:

- **provider**: Java flavor to use. Possible options are `oracle` or `openjdk`
- **version**: Default Java version. Possible options 6, 7 or 8 (OpenJDK) and 8 or 9 (Oracle Java)

```
java_default_alternative:
  provider: openjdk
  version: 8
```

## Dependencies

None.

## Example Playbook

    - hosts: all
      roles:
        - T2L.java

## License

MIT

## Author Information

This role was created in 2017 by Roman Paska.

## Changelog

Changelog can be found here [CHANGELOG.md](CHANGELOG.md)
