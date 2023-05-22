# gnome

[![Source Code](https://img.shields.io/badge/github-source%20code-blue?logo=github&amp;logoColor=white)](https://github.com/rolehippie/gnome)
[![General Workflow](https://github.com/rolehippie/gnome/actions/workflows/general.yml/badge.svg)](https://github.com/rolehippie/gnome/actions/workflows/general.yml)
[![Readme Workflow](https://github.com/rolehippie/gnome/actions/workflows/readme.yml/badge.svg)](https://github.com/rolehippie/gnome/actions/workflows/readme.yml)
[![Galaxy Workflow](https://github.com/rolehippie/gnome/actions/workflows/galaxy.yml/badge.svg)](https://github.com/rolehippie/gnome/actions/workflows/galaxy.yml)
[![License: Apache-2.0](https://img.shields.io/github/license/rolehippie/gnome)](https://github.com/rolehippie/gnome/blob/master/LICENSE)
[![Ansible Role](https://img.shields.io/badge/role-rolehippie.gnome-blue)](https://galaxy.ansible.com/rolehippie/gnome)

Ansible role to install and configure Gnome related stuff.

## Sponsor

Building and improving this Ansible role have been sponsored by my current and previous employers like **[Cloudpunks GmbH](https://cloudpunks.de)** and **[Proact Deutschland GmbH](https://www.proact.eu)**.

## Table of content

- [Requirements](#requirements)
- [Default Variables](#default-variables)
  - [gnome_extra_plugins](#gnome_extra_plugins)
  - [gnome_extra_themes](#gnome_extra_themes)
  - [gnome_general_plugins](#gnome_general_plugins)
  - [gnome_general_themes](#gnome_general_themes)
- [Discovered Tags](#discovered-tags)
- [Dependencies](#dependencies)
- [License](#license)
- [Author](#author)

---

## Requirements

- Minimum Ansible version: `2.10`


## Default Variables

### gnome_extra_plugins

#### Default value

```YAML
gnome_extra_plugins: []
```

### gnome_extra_themes

#### Default value

```YAML
gnome_extra_themes: []
```

### gnome_general_plugins

#### Default value

```YAML
gnome_general_plugins: []
```

### gnome_general_themes

#### Default value

```YAML
gnome_general_themes:
  - name: Nordic-v40
    url: https://github.com/EliverLara/Nordic/releases/download/v2.2.0/Nordic-v40.tar.xz
```

## Discovered Tags

**_gnome_**


## Dependencies

- [rolehippie.docker](https://github.com/rolehippie/docker)

## License

Apache-2.0

## Author

[Thomas Boerger](https://github.com/tboerger)
