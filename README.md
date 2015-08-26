# Apt Cacher

## Host Server

This playbook is written for deployment on an Ubuntu 14.04 LTS server, that can
be accessed from all clients within the network. The server is designated in the
[`hosts`](hosts.example) file under the `[server]` group.

## Clients

Any computer running APT as a package manager can be configured to use the Apt
Cache found on the server. Clients should be listed in the [`hosts`](hosts.example)
file under the `[clients]` group.

## Configuration

In the [`vars/main.yml`](vars/main.yml.example) file, change the `host_domain`
to the domain or IP address that has been allocated for your `server`.
