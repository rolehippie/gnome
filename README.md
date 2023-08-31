# gnome

[![Source Code](https://img.shields.io/badge/github-source%20code-blue?logo=github&logoColor=white)](https://github.com/rolehippie/gnome)
[![General Workflow](https://github.com/rolehippie/gnome/actions/workflows/general.yml/badge.svg)](https://github.com/rolehippie/gnome/actions/workflows/general.yml)
[![Readme Workflow](https://github.com/rolehippie/gnome/actions/workflows/docs.yml/badge.svg)](https://github.com/rolehippie/gnome/actions/workflows/docs.yml)
[![Galaxy Workflow](https://github.com/rolehippie/gnome/actions/workflows/galaxy.yml/badge.svg)](https://github.com/rolehippie/gnome/actions/workflows/galaxy.yml)
[![License: Apache-2.0](https://img.shields.io/github/license/rolehippie/gnome)](https://github.com/rolehippie/gnome/blob/master/LICENSE)
[![Ansible Role](https://img.shields.io/badge/role-rolehippie.gnome-blue)](https://galaxy.ansible.com/rolehippie/gnome)

Ansible role to install and configure Gnome related stuff.

## Sponsor

Building and improving this Ansible role have been sponsored by my current and previous employers like **[Cloudpunks GmbH](https://cloudpunks.de)** and **[Proact Deutschland GmbH](https://www.proact.eu)**.

## Table of content

- [Requirements](#requirements)
- [Default Variables](#default-variables)
  - [gnome_extra_icons](#gnome_extra_icons)
  - [gnome_extra_packages](#gnome_extra_packages)
  - [gnome_extra_plugins](#gnome_extra_plugins)
  - [gnome_extra_themes](#gnome_extra_themes)
  - [gnome_general_icons](#gnome_general_icons)
  - [gnome_general_packages](#gnome_general_packages)
  - [gnome_general_plugins](#gnome_general_plugins)
  - [gnome_general_themes](#gnome_general_themes)
  - [gnome_updated_icon_cache](#gnome_updated_icon_cache)
- [Discovered Tags](#discovered-tags)
- [Dependencies](#dependencies)
- [License](#license)
- [Author](#author)

---

## Requirements

- Minimum Ansible version: `2.10`

## Default Variables

### gnome_extra_icons

List of extra icons to install globally

#### Default value

```YAML
gnome_extra_icons: []
```

#### Example usage

```YAML
gnome_extra_icons:
  - name: Nordic-v40
    url: https://github.com/EliverLara/Nordic/releases/download/v2.2.0/Nordic-v40.tar.xz
  - name: foobar
    state: absent
```

### gnome_extra_packages

List of extra packages to install

#### Default value

```YAML
gnome_extra_packages: []
```

#### Example usage

```YAML
gnome_extra_packages:
  - gnome-calendar
  - name: gnome-foobar
    state: absent
```

### gnome_extra_plugins

List of extra extensions to install globally

#### Default value

```YAML
gnome_extra_plugins: []
```

#### Example usage

```YAML
gnome_extra_plugins:
  - name: user-theme
    id: user-theme@gnome-shell-extensions.gcampax.github.com
```

### gnome_extra_themes

List of extra themes to install globally

#### Default value

```YAML
gnome_extra_themes: []
```

#### Example usage

```YAML
gnome_extra_themes:
  - name: Nordic-v40
    url: https://github.com/EliverLara/Nordic/releases/download/v2.2.0/Nordic-v40.tar.xz
  - name: foobar
    state: absent
```

### gnome_general_icons

List of general icons to install globally

#### Default value

```YAML
gnome_general_icons:
  - name: Nordzy-Cursors
    url: 
      https://github.com/alvatip/Nordzy-cursors/releases/download/v0.6.0/Nordzy-cursors.tar.gz
    opts:
      - --transform
      - s/^Nordzy-cursors/Nordzy-Cursors/
  - name: Nordzy-Icons
    url: https://github.com/alvatip/Nordzy-icon/releases/download/1.8.5/Nordzy.tar.gz
    opts:
      - --transform
      - s/^Nordzy/Nordzy-Icons/
```

#### Example usage

```YAML
gnome_general_icons:
  - name: Nordic-v40
    url: https://github.com/EliverLara/Nordic/releases/download/v2.2.0/Nordic-v40.tar.xz
  - name: foobar
    state: absent
```

### gnome_general_packages

List of general packages to install

#### Default value

```YAML
gnome_general_packages: []
```

#### Example usage

```YAML
gnome_general_packages:
  - gnome-calendar
  - name: gnome-foobar
    state: absent
```

### gnome_general_plugins

List of general extensions to install globally

#### Default value

```YAML
gnome_general_plugins: []
```

#### Example usage

```YAML
gnome_general_plugins:
  - name: user-theme
    id: user-theme@gnome-shell-extensions.gcampax.github.com
```

### gnome_general_themes

List of general themes to install globally

#### Default value

```YAML
gnome_general_themes:
  - name: Nordic
    url: https://github.com/EliverLara/Nordic/releases/download/v2.2.0/Nordic-v40.tar.xz
    opts:
      - --transform
      - s/^Nordic-v40/Nordic/
```

#### Example usage

```YAML
gnome_general_themes:
  - name: Nordic-v40
    url: https://github.com/EliverLara/Nordic/releases/download/v2.2.0/Nordic-v40.tar.xz
  - name: foobar
    state: absent
```

### gnome_updated_icon_cache

Update the GTK icon cache

#### Default value

```YAML
gnome_updated_icon_cache: true
```

## Discovered Tags

**_gnome_**


## Dependencies

- [rolehippie.docker](https://github.com/rolehippie/docker)

## License

Apache-2.0

## Author

[Thomas Boerger](https://github.com/tboerger)
