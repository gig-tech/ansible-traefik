traefik
=========

[![Build Status](https://travis-ci.org/jebovic/ansible-traefik.svg?branch=master)](https://travis-ci.org/jebovic/ansible-traefik)

Role Variables
--------------

```yaml
# Traefik installation configuration
traefik_install_dir: /usr/local/bin
traefik_binary_url: https://github.com/containous/traefik/releases/download/v1.7.11/traefik_linux-amd64
traefik_bin_path: "{{ traefik_install_dir }}/traefik"
traefik_config_dir: /etc/traefik

traefik_static_config: |
                        # Add your custom static config here

traefik_dynamic_config: |
                        # Add your custom dynamic config here
```

Example Playbook
----------------

```yaml
- hosts: servers
  roles:
     - { role: gig.tech.traefik }
```

License
-------

MIT

Author Information
------------------

GIG Technology NV https://github.com/gig-tech
