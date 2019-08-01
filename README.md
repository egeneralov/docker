egeneralov.docker
=================

Docker daemon provision with configuration.

Requirements
------------

- debian-based system

Role Variables
--------------

See `defaults/main.yml`.

- **docker_download_url**: `https://download.docker.com/linux/{{ ansible_distribution | lower }}`
- **docker_release_channel**: `stable` (edge / stable)
- **docker_type**: `ce` (ce / ee)
- **docker_version**: `present`
  - present
  - 18.06.3~ce~3-0~debian
  - latest
- **docker_compose_version**: `1.23.2`
  - recommend to keep version. 1.24.{0,1} has bugs
- **docker_registry**: `[]`
  - **url**: `registry-1.docker.io` (optional, default - hub.docker.com)
    **username**: `egeneralov` (username)
    **password**: `egeneralov` (password)
- **docker_daemon_json**: `{}` (map for daemon.json)

License
-------

MIT
