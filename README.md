docker-dnsmasq
==============

This is part of [mayfly](https://github.com/bewt85/mayfly) which demonstrates the 
concept of testing groups of versions of services in short lived virtual environments.

This is a docker container which uses incrond to reload itself whenever `/etc/dnsmasq/hosts` 
changes. It is updated by [dnsmasq_updater](https://github.com/bewt85/mayfly-dnsmasq-updater) 
which mounts the `/etc/dnsmasq` folder.

You can build your own version of the container by setting the following environment variable 
to your docker index username (if you don't it uses mine) and running this bash script:

```
export DOCKER_ACCOUNT_NAME=<your_name>
sudo -E ./build.sh
```
