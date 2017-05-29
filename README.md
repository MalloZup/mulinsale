# Mulinsale

This repo contains various docker imgs for salt-minions.

### for testing:

remove machine-id
```console
docker run noiz /bin/bash -c "dbus-uuidgen > /etc/machine-id; salt-minion -l trace"
```
