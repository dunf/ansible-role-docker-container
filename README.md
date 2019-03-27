Ansible Role: Docker container
=========

Pull/Build docker containers and run them. Build functionality is not yet added

Requirements
------------

None

Role Variables
--------------
Available variables are listed below, along with default values (see defaults/main.yml):

```
image
```
Path to the image in docker hub. Must be defined

```
container_name
```
The name given to the container. Must be defined

```
public_port
```
The port that is exposed to the host. Must be defined

```
pull
```
Whether or not to always pull the latest version of the image. `Default: yes` 



Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: docker-container, image: foo:latest, container_name: bar, public_port: 1337 }

License
-------

MIT

