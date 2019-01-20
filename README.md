egeneralov.docker
=========

Docker daemon provision with configuration.

Requirements
------------

- debian-based system

Role Variables
--------------

- download_url, string, base url for download.docker.com
- registry, list with map
  - url, string, registry host
  - username, string
  - password, string
- dns, list, with ip strings
- max_concurrent_downloads, int, max concurent streams for pulling images
- max_concurrent_uploads, int, max concurent streams for pushing images
- insecure_registries, list, with strings of insecure registry hosts
- log_opts, map, options for daemon.json


License
-------

MIT
