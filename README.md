# Helm Chart for Papermerge

This is helm chart for Papermerge deployment in Kubernetes cluster.


## Install

In order to install papermerge use following command:

    helm install papermerge . -f .values.yaml

## Parameters

### Worker parameters

| Name                  | Description                     | Value |
| --------------------- | ------------------------------- | ----- |
| `worker.replicaCount` | Amount of worker pods to create | `3`   |


### Global parameters

| Name                                     | Description                          | Value                 |
| ---------------------------------------- | ------------------------------------ | --------------------- |
| `global.conf.app.django_settings_module` |                                      | `config.settings`     |
| `global.conf.app.superuser.username`     | Django SuperUser username            | `admin`               |
| `global.conf.app.superuser.email`        | Django SuperUser email               | `admin@example.com`   |
| `global.conf.app.media_dir`              | Default location for all media files | `/app/media`          |
| `global.conf.app.logging_config`         |                                      | `""`                  |
| `global.conf.app.tz`                     |                                      | `GMT`                 |
| `global.conf.ingress.enabled`            | Enables the ingress module           | `true`                |
| `global.conf.ingress.host`               | Host name of ingress thing           | `papermerge.minikube` |
| `global.conf.db.type`                    | Database engine type                 | `postgres`            |
| `global.conf.db.user`                    | Database login user                  | `postgres`            |
| `global.conf.db.name`                    | Database name                        | `postgres`            |
| `global.conf.db.host`                    | Hostname of database                 | `db`                  |
| `global.conf.db.port`                    | Port for database                    |                       |
| `global.conf.es.enabled`                 |                                      | `false`               |
| `global.conf.es.host`                    |                                      |                       |
| `global.conf.es.port`                    |                                      |                       |
| `global.conf.redis.host`                 | Host name of redis service           | `redis`               |
| `global.conf.redis.port`                 | Port of redis service                | `6379`                |
| `global.secrets.db.password`             |                                      | `""`                  |
| `global.secrets.app.secret_key`          |                                      | `""`                  |
| `global.secrets.app.superuser.password`  |                                      | `""`                  |

