## Ansible Role: Java 1.x.x

- Dropped support of Oracle Java 11 (cannot be used without an Oracle account) and replaced it with Oracle Java 13
- Add support for OpenJDK 12 and 13 (not for all Ubuntu versions)

## Ansible Role: Java 1.1.0, 2018-10-24

- Bump minimum Ansible version to 2.5
- Fixed _Invoking "apt" only once while using a loop via squash_actions is deprecated._
- Added support for Ubuntu 18.04
- Use `loop` keyword instead of `with_<lookup>`
- Dropped support of Oracle Java 9 (reached EOL) and replaced it with Oracle Java 11 (LTS release)

## Ansible Role: Java 1.0.0, 2017-07-03

- Initial release
