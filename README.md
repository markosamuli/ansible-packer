# ansible-packer

[![Build Status](https://travis-ci.org/markosamuli/ansible-packer.svg?branch=master)](https://travis-ci.org/markosamuli/ansible-packer)

Ansible role to install [Packer](https://www.packer.io/) on Ubuntu and macOS.

Used in the Ansible playbooks for setting up my workstations:

- [markosamuli/machine](https://github.com/markosamuli/machine)
- [markosamuli/linux-machine](https://github.com/markosamuli/linux-machine)
- [markosamuli/macos-machine](https://github.com/markosamuli/macos-machine)

## macOS

On macOS, Homebrew [packer formula](https://formulae.brew.sh/formula/packer) is used.

## Linux

On Ubuntu, packer binary is installed into `/opt/packer` and symlink created 
in `/usr/local/bin`.

To change installed version, update the version and checksum:

```yaml
packer_version: "1.3.2"
packer_checksum: "sha256:5e51808299135fee7a2e664b09f401b5712b5ef18bd4bad5bc50f4dcd8b149a1"
```

See [Packer Downloads](hhttps://www.packer.io/downloads.html) page for latest
version and checksum.

## License

MIT
