# Ansible Role: jeffhung.maven

Ansible playbook for installing Maven on CentOS/Debian Linux

Install this playbook:

	ansible-galaxy install jeffhung.maven


## Role Variables

### `maven_version`

Default: `2.2.1`

Set which Maven version to use.

### `maven_environment`

Default: `devel`

Which environment to deploy.

Could be:

* `devel`: provision devel-time environment for developing with Maven
* `build`: provision build-time environment for packaging Maven

### `maven_install_from`

Choose the source where maven is installed from.

Could be:

* `binaries`: install from binary tarball released by Apache
* `packages`: install from automatically downloaded RPM/DEB packages
* `repositories`: install from jpackage YUM/APT repositories

Default: `binaries`


### `maven_cache_dir`

Cache directory for holding downloaded/generated files.

The default is `/vagrant/files` so cache persist between boxes.


## License

BSD

