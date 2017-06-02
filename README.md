# Mulinsale

This repo contains various docker imgs for salt-minions.

### building


#### run

```console 
MASTER=`cat /etc/salt/minion.d/susemanager.conf` ;
docker run -d--entrypoint '/bin/sh' rhel6 -c "echo $MASTER > /etc/salt/minion; dbus-uuidgen > /etc/machine-id; salt-minion -l trace"

```




### for testing:

remove machine-id
```console
docker run noiz /bin/bash -c "dbus-uuidgen > /etc/machine-id; salt-minion -l trace"
```
