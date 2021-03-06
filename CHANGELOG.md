## Ansible Role: Java 1.3.3, 2021-04-12

- [#21](https://github.com/T2L/ansible-role-java/issues/21) - Oracle Java 15 is no longer supported, replaced it with version 16
- Explicitly require yamllint on Travis CI

## Ansible Role: Java 1.3.2, 2021-03-11

- [#20](https://github.com/T2L/ansible-role-java/pull/20) - Make Travis CI green again
- [#16](https://github.com/T2L/ansible-role-java/issues/18) - Oracle Java 14 is no longer supported, replaced it with version 15

## Ansible Role: Java 1.3.1, 2020-08-20

- [#16](https://github.com/T2L/ansible-role-java/issues/16) - Address newly introduced Ansible Lint "[208] File permissions not mentioned" message. Update Travis configuration (new Ansible version)

## Ansible Role: Java 1.3.0, 2020-04-27

- [#13](https://github.com/T2L/ansible-role-java/issues/13) - Add Ubuntu 20.04 support
- [#11](https://github.com/T2L/ansible-role-java/issues/11) - OpenJDK 13 is no longer supported, replaced with JDK 14
- [#9](https://github.com/T2L/ansible-role-java/issues/9) - Add Molecule 3 support

## Ansible Role: Java 1.2.0, 2020-01-11

- Dropped support of Oracle Java 11 (cannot be used without an Oracle account) and replaced it with Oracle Java 13
- Add support for OpenJDK 12 and 13 (not for all Ubuntu versions)
- Set OpenJDK Java 11 JRE as default
- Fix Ansible deprecation warning:

  ```
  [DEPRECATION WARNING]: evaluating X as a bare variable, this behaviour will go away and you might need to add |bool to the expression in the future.
  ```

## Ansible Role: Java 1.1.0, 2018-10-24

- Bump minimum Ansible version to 2.5
- Fixed _Invoking "apt" only once while using a loop via squash_actions is deprecated._
- Added support for Ubuntu 18.04
- Use `loop` keyword instead of `with_<lookup>`
- Dropped support of Oracle Java 9 (reached EOL) and replaced it with Oracle Java 11 (LTS release)

## Ansible Role: Java 1.0.0, 2017-07-03

- Initial release
