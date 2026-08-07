# runit-services

> Runit service scripts for Gentoo Linux

[![Gentoo](https://img.shields.io/badge/Gentoo-54487A?style=flat&logo=gentoo&logoColor=white)](https://www.gentoo.org/)
[![runit](https://img.shields.io/badge/init-runit-blue)](http://smarden.org/runit/)
[![License](https://img.shields.io/badge/license-MIT-blue)](LICENSE)

---

## Contents

- [Installation](#installation)
- [Enabling a service](#enabling-a-service)

---

## Installation

[Enable the runit-overlay](https://github.com/gentoo-runit/runit-overlay#installation)


---

## Enabling a service

Installing a service directory does not activate it. Symlink it into the scan directory once you're ready:

```bash
ln -s /etc/sv/dbus /etc/service/
```

Removing the symlink stops and disables it; runit notices the directory disappearing and tears the supervised process down.
